# Curiosity Report

One thing that I found pretty interesting in this course is the extensive use of GitHub actions. It's clearly very useful and well integrated with GitHub, but I wondered how it stacks up to Jenkins. I've used Jenkins before, but I've never really considered the differences between the two and decided which I prefer (although it's likely I'll just end up using whatever is already being used wherever I am). Thus, this curiosity report was born.

## Differences

I'd say that the biggest difference between the two is that GitHub actions can be run by GitHub itself, while Jenkins can only be hosted by you or another third party. This has several effects.

 1. Support is built into your GitHub repo, you simply need to use it. Meanwhile, Jenkins must be set up.
 2. You can use actions all in the same website as where you manage your repo.
 3. Jenkins can be used with other git repos, such as gitlab, while actions requires some finagling. In my research, it seems like it's possible to use GitHub actions outside of GitHub , but it's unlikely that support is anywhere near as good.
 4. For extremely security conscious people, this benefit to GitHub actions doesn't matter, as they are likely to want to host their own instance of either.
 5. If you use github's instance of actions, for huge projects it can end up costing more than self hosting.

 This results in GitHub actions being far easier to get started with as a beginner, but not particularly having huge benefits for those who might be security conscious or running huge projects.
 It's probably not a huge consideration for most people, but GitHub actions, while partially open source, has some parts that are closed source, making it less open source than Jenkins.

## Opinion

Having used both, I'd say that I like the developer experience for GitHub actions a lot more. Just the way that everything seamlessly connects with the repo is really nice. While it didn't happen with Jenkins, deciding to use Jenkins means committing to managing that part of your pipeline yourself. This means it can break at any time, and you'd have to be the one to fix it. In terms of a company, it means that you probably need to have a whole team dedicated to making sure that everything runs smoothly (though this is probably already handled by devops, you can probably save on hiring some people without Jenkins). For my use cases as a single developer, I'd definitely choose actions for any project that I'm doing.

Even though it's not a super great reason, I remember that with Jenkins, I had to have a million tabs open all the time. Being able to access everything inside of GitHub is an underrated, but important consideration for me. That being said, for someone who is more familiar with Java, they might choose Jenkins, as it uses Groovy. Really, they seem to be pretty feature complete, so it's up to the developer to choose whatever they're most comfortable with.
