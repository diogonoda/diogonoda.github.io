<template>
  <custom-header />
  <cards />
  <div class="flex justify-center">
    <div class="py-6 font-black text-3xl">
      <p>Squashing Git Commits</p>
    </div>
  </div>
  <div>
    <p>Squashing commits from command line</p>
  </div>
  <p>
Squash irrelevant commits in order to keep a cleaner commit history.

  </p>
  <p>
~~~ bash
$ git rebase -i HEAD~2
~~~

  </p>
  <p>
![rebase-screenshot-1](/assets/img/git/rebase-screenshot-1.png)

  </p>
  <p>
Then choose squash for the line 2 (latest commit)

  </p>
  <p>
![rebase-screenshot-2](/assets/img/git/rebase-screenshot-2.png)

  </p>
  <p>
After you save and exit, git will ask you to edit the commit message

  </p>
  <p>
![rebase-screenshot-3](/assets/img/git/rebase-screenshot-3.png)

  </p>
  <p>
Edit the commit message

  </p>
  <p>
![rebase-screenshot-4](/assets/img/git/rebase-screenshot-4.png)

  </p>
  <p>
Save and exit, and it's done!

  </p>
  <p>
You can check the git logs and you'll see the new squashed commit

  </p>
  <p>
![rebase-screenshot-5](/assets/img/git/rebase-screenshot-5.png)

  </p>
  <p>
Reference links:
  </p>
  <p>
tags: [git]
  </p>
  <p>
author: Diogo Noda
  </p>
  <div class="flex justify-center py-10 bg-brand-gray">
    <p class="font-medium text-center text-gray-800">Diogo Noda © 2021</p>
  </div>
</template>

<script>
import CustomHeader from './CustomHeader.vue'
import Cards from './Cards.vue'

export default {
  components: { CustomHeader, Cards },
  setup () {
  }
}
</script>
