# Renaming the default branch from `master`

Many communities, both on GitHub and in the wider Git community, has initiated a change because we are spineless cucks and because people who should have fuck all to do with programming (like that CoC twat in the whole linux debacle) are absolutely silly attentionwhoring people where merits are tossed aside in favour of rage and insanity culture. Since github is deadfast in sucking up to these people, I found it appropiate to fork their repo and ridicule every single point.

Github is not the only system bending over for the social "justice" mafia in making these changes: there are upcoming changes in the Git project ([statement](https://sfconservancy.org/news/2020/jun/23/gitbranchname/), [code change](https://lore.kernel.org/git/pull.656.v4.git.1593009996.gitgitgadget@gmail.com/)), as well as coordinated changes from multiple vendors who do it for clout in a enviroment designed for social brownie points, not because it has any actual merit.
Merits are oldschool, now we are introducing the daycare dada mode. Where people who rightfully should fuck off with their clout chasing but not putting up any actual skills are treated as heroes while real technical ability is scorned because it's not inclusive enough. Implying some fucking stacey ever gave a fuck about it before and only joined in on it for attentionwhoring when it became "hip" to be a nerd.

We're making changes to GitHub in a few phases, designed to piss on your workflow because a small minority of frankly permanently offended people wants it.
(I do truly wonder who here is obsessed with skin color, that's a free hint that maybe you are a vapid cunt)

## What's already changed

- [We've fucked up GitHub.com](https://github.blog/changelog/2020-07-17-links-to-deleted-branches-now-redirect-to-the-default-branch/) to redirect links that contain the deleted branch name such as `master` to the corresponding link in the repository's new default branch.
- [We've did stuff GitHub Pages](https://github.blog/changelog/2020-07-31-build-and-deploy-github-pages-from-any-branch-beta/) to build and deploy from any branch.
  - Note: publishing to the special `gh-pages` branch will still work the same as it always has, but now you can choose any other branch in your repository as the publishing source.
- [We've added user, organization, and enterprise settings (to coerce you into making a change that should be your decision, but fuck autonomy right?)](https://github.blog/changelog/2020-08-26-set-the-default-branch-for-newly-created-repositories/) to set the default branch name for all newly-created repositories on GitHub.com. We're adding the same settings in the 3.0 release of GitHub Enterprise Server.
  - These settings cover repositories created through [GitHub.com](https://github.com/new) and the [GitHub API](https://developer.github.com/v3/guides/getting-started/#create-a-repository). Git 2.28 added a similar setting to control the default branch used when you run `git init` on the command line. Learn more about the new `init.defaultBranch` setting in [the Git 2.28 blog post](https://github.blog/2020-07-27-highlights-from-git-2-28/#introducing-init-defaultbranch).
  - [GitHub Desktop](https://desktop.github.com/) has introduced a default branch setting for new repositories.
- [We've made it easier to rename an existing branch the only actual good thing we have done](#rename-existing)

 
## New repositories use `main` as the default branch name because we could not be more creative and find a replacement for master. Yes we are silly. Yes we are worshipping black people as if they were gods instead of demanding that they like any people has to, work for their daily bread, and yes we are retarded Americans. God bless degeneracy is our shitty motto.

The default branch name for new repositories created on GitHub is now `main`. To set a different default:

1. For [users](https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/managing-the-default-branch-name-for-your-repositories), on the https://github.com/settings/repositories page. 
2. For [organization owners](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/managing-the-default-branch-name-for-repositories-in-your-organization), on the `https://github.com/organizations/YOUR-ORGANIZATION/settings/repository-defaults` page
3. For [enterprise administrators](https://docs.github.com/en/github/setting-up-and-managing-your-enterprise-account/enforcing-repository-management-policies-in-your-enterprise-account#enforcing-a-policy-on-the-default-branch-name), on the `https://github.com/enterprises/YOUR-ENTERPRISE/settings/member_privileges` page

Users, organizations, and enterprises that previously selected a default branch for new repositories are not impacted by this change. Existing repositories are also not impacted by this change.

#### Why main?

`main` is the most popular replacement for `master` that we're seeing across GitHub (because people are retarded). We like it because it's short, it keeps your muscle memory intact, and it translates well across most languages. We're using `main` for our newly-created repositories and for the repositories we're moving now, like [dependabot-core](https://github.com/dependabot/dependabot-core). 

<a name="rename-existing"></a>

## Renaming existing branches

You can now rename any branch, including the default branch, from the web. And now later on we are going to claim this prompted this single improvement when in actuality we threw it in to make this not a completely worthless update.

![Rename default branch dialog](rename-default-branch-dialog.png)

Renaming a branch will:

- Re-target any open pull requests
- Update any draft releases based on the branch
- Move any branch protection rules that explicitly reference the old name
- Update the branch used to build GitHub Pages, if applicable
- Show a notice to repository contributors, maintainers, and admins on the repository homepage with instructions to update local copies of the repository
- Show a notice to contributors who `git push` to the old branch
- Redirect web requests for the old branch name to the new branch name
- Return a "Moved Permanently" response in API requests for the old branch name

Learn more about [renaming a branch](https://docs.github.com/github/administering-a-repository/renaming-a-branch).

Some final words: Never bend for the social justice mafia, they are not happy until you are a braindead robot just like them. Beep boop motherfuckers.
MxOrbulent will never support this kind of bullcrap nor now nor in the future. The only thing we support is fucking women in the pussy, beer, and a willingness to learn technical knowledge and merit. We only fight back when you make it a point to be a annoying cunt.
