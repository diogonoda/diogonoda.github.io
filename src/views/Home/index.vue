<template>
  <custom-header />
  <cards />
  <p>
Squashing Git Commits
Squashing commits from command line

Squash irrelevant commits in order to keep a cleaner commit history.

~~~ bash
$ git rebase -i HEAD~2
~~~

![rebase-screenshot-1](/assets/img/git/rebase-screenshot-1.png)

Then choose squash for the line 2 (latest commit)

![rebase-screenshot-2](/assets/img/git/rebase-screenshot-2.png)

After you save and exit, git will ask you to edit the commit message

![rebase-screenshot-3](/assets/img/git/rebase-screenshot-3.png)

Edit the commit message

![rebase-screenshot-4](/assets/img/git/rebase-screenshot-4.png)

Save and exit, and it's done!

You can check the git logs and you'll see the new squashed commit

![rebase-screenshot-5](/assets/img/git/rebase-screenshot-5.png)

Reference links:
tags: [git]
author: Diogo Noda
  </p>
  <div class="flex justify-center py-10 bg-brand-gray">
    <p class="font-medium text-center text-gray-800">Diogo Noda © 2021</p>
  </div>
</template>

<script>
import CustomHeader from './CustomHeader.vue'

export default {
  components: { CustomHeader },
  setup () {
  }
}
</script>
