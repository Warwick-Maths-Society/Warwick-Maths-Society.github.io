# Warwick Maths Society Website

[![Current Version](https://img.shields.io/github/tag/Warwick-Maths-Society/Warwick-Maths-Society.github.io.svg)](https://github.com/Warwick-Maths-Society/Warwick-Maths-Society.github.io/tags)
[![Discord](https://img.shields.io/discord/1102960469934870560.svg)](https://discord.gg/UWrqB93gfh)
[![Open Issues](https://img.shields.io/github/issues/Warwick-Maths-Society/Warwick-Maths-Society.github.io.svg)](https://github.com/Warwick-Maths-Society/Warwick-Maths-Society.github.io/issues)
[![Contributors](https://img.shields.io/github/contributors/Warwick-Maths-Society/Warwick-Maths-Society.github.io.svg)](https://github.com/Warwick-Maths-Society/Warwick-Maths-Society.github.io/pulse/monthly)
[![pages-build-deployment](https://github.com/Warwick-Maths-Society/Warwick-Maths-Society.github.io/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/Warwick-Maths-Society/Warwick-Maths-Society.github.io/actions/workflows/pages/pages-build-deployment)

This is the official website for the Warwick Maths Society.

You can add posts or request changes by making a fork of the `main` branch and opening a [pull request](https://github.com/Warwick-Maths-Society/Warwick-Maths-Society.github.io/pulls).

The sources for the essay, module review, exec, etc., pages can be found in the [_pages](_pages) directory.



# Maintainers

This website is developed and maintained by [Kit Liu](https://github.com/DesyncTheThird), with various content contributions (module reviews, essays, etc.) from the wider WMS community.

Maintenance will be taken over by the Publications Officer once one is elected.



# Contributing

Thank you for looking in to contributing!

You do not need to install anything to contribute; in this case, you will not be able to preview your changes, and you should indicate that this is the case in your pull request.
That is, you should tick the second box in the last section of the pull request template:

> - [ ] I have built and tested these changes locally or otherwise, and confirm that they work and don't break existing functionality.
> - [x] I have not built these changes locally or otherwise, and require someone to review these changes for me.

## Previewing Changes

If you would like to preview your changes, you will need to install [Ruby](https://www.ruby-lang.org/en/documentation/installation/) and [Jekyll](https://jekyllrb.com/docs/installation/) in order to build your site locally.

---

### Windows

<details>
<summary>Instructions</summary>
  
1. [Install Ruby](https://rubyinstaller.org/downloads/).
   * Run `ridk install` on the last step of the installer and choose `MSYS2 and MINGW development toolchain` when prompted.
   * Alternatively, you can use WinGet:
   
     ``` shell
     winget install RubyInstallerTeam.RubyWithDevKit.3.2
     ```
     
     or chocolatey:
     
     ``` shell
     choco install ruby2.devkit
     ```
     
     if you already have a package manager.
3. [Install RubyGems](https://rubygems.org/pages/download).
4. Open a new terminal and run:

   ```shell
   gem install jekyll bundler
   ```

5. Verify that your installation is working by running:

   ```shell
   jekyll -v
   ```

</details>



### MacOS

<details>
<summary>Instructions</summary>

1. Install the version manager `chruby` and `ruby-install` with:

   ```shell
   brew install chruby ruby-install
   ```

3. Install the latest version of Ruby supported by Jekyll with:

   ```shell
   ruby-install ruby 3.3.5
   ```

4. Then configure your terminal to use `chruby` with:

   ```shell
   echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
   echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
   echo "chruby ruby-3.3.5" >> ~/.zshrc # run 'chruby' to see actual version
   ```

3. Open a new terminal and run:

   ```shell
   gem install jekyll bundler
   ```

4. Verify that your installation is working by running:

   ```shell
   jekyll -v
   ```

</details>



### VSCode Setup

<details>
<summary>Instructions</summary>
<br/>
  
1. Install the [Jekyll Run](https://marketplace.visualstudio.com/items?itemName=Dedsec727.jekyll-run) extension.
   * Optionally also install the [Jekyll Syntax Support](https://marketplace.visualstudio.com/items?itemName=ginfuru.ginfuru-vscode-jekyll-syntax) extension.
2. Press `Ctrl`+`Shift`+`P` and type in `Jekyll` until the following commands appear:
   * Run `Jekyll: Build`;
   * Run `Jekyll: Run`.
3. In the `Output` panel, you should see the site building. After a short delay (usually 8-12 seconds), you should be able to see your site live at `localhost:4000`.

If you would like to use the Tasks feature to build your site, add:

```json
{
    "version": "2.0.0",
    "tasks": [
        {
            "label": "Start Jekyll",
            "type": "shell",
            "command": "bundle exec jekyll serve --host localhost --port 4000",
            "group": {
            "kind": "build",
            "isDefault": true
            }
        }
    ]
}
```

to your `tasks.json`.

</details>

---

> ⚠️ When editing your post/review/other page contribution, make sure that you are editing a `.md` source file, and not an `.html` file generated by Jekyll.



## Module Reviews

The module review page may be found [here](_pages/module_reviews.md).

Each module review will look something like this:

```html
<!-- -->
<div class="card-header" id="headingMAXYZ">
  <h2 class="m-0">
    <button class="btn btn-link btn-block text-left" type="button" data-toggle="collapse" data-target="#collapseMAXYZ" aria-expanded="false" aria-controls="collapseMAXYZ" id="MAXYZ"
    disabled>
      <large><a href="#MAXYZ">MAXYZ Module Name</a></large>
    </button>
  </h2>
</div>
<div id="collapseMAXYZ" class="collapse" aria-labelledby="headingMAXYZ" data-parent="#accordionY3maths">
  <div class="card-body">
    <large class="text-muted">YY/YY</large>
    <br/>
    review here
  </div>
</div>
<!-- -->
```

with empty comment lines marking the boundaries of each review.

If a review does not already exist:
1. Replace the `review here` line with the review. See existing reviews for formatting conventions.
2. Delete the `disabled` attribute from the button (which is helpfully written on a separate line).

> ⚠️ Do not remove the closing angle bracket (`>`); just move this to the end of the line above to keep things neat.

If a review already exists:
1. Add two new lines (`<br/>`) **above** the year line of the **highest** older review at the top of the list.
2. Stack the new review on top (including adding a copy of the year line), formatting the new review as usual.

That is:

```html
<div id="collapseMAXYZ" class="collapse" aria-labelledby="headingMAXYZ" data-parent="#accordionY3maths">
  <div class="card-body">
    <large class="text-muted">22/23</large>
    <br/>
    This is my old review. It is old.
  </div>
</div>
```
should turn into:

```html
<div id="collapseMAXYZ" class="collapse" aria-labelledby="headingMAXYZ" data-parent="#accordionY3maths">
  <div class="card-body">
    <large class="text-muted">23/24</large>
    <br/>
    This is my new review. It is new.
    <br/>
    <br/>
    <large class="text-muted">22/23</large>
    <br/>
    This is my old review. It is old.
  </div>
</div>
```

## Essay Contributions

To contribute your essay

1. Rename your essay file in the following format:

   ```shell
   [mark] - [full essay name].pdf
   ```

> ⚠️ Your file must be a PDF.

2. Copy it into `assets/essay-2` or `assets/essay-3`, depending on whether it is a second or third year essay.

3. Navigate to the [essay page](_pages/essays.md).

4. In the appropriate table, add the following lines:

   ```html
   <tr>
     <td>[mark]</td>
     <td><a target="_blank" href="./assets/essays-[2|3]/
   [mark] - [full essay name].pdf">[full essay name]</a></td>
   </tr>
   ```

   replacing each field as required.


## Posts

> ℹ️ This section should only be relevant to Exec or other authorised persons; pull requests for unauthorised posts will be closed without discussion.

The template for new posts (`YYYY-MM-DD-template.md`) can be found [here](_posts/YYYY-MM-DD-template.md), and quick reference sheets for markdown/kramdown can be found [here](_cheatsheet) (or [live](https://warwick-maths-society.github.io/cheatsheets)). New posts should be placed in the [_pages](_pages) directory (i.e. the same folder as the post template).

Rename your copy of the template post in the following format `YYYY-MM-DD-<name>.md`, and see the included instructions for more details.

Place any files that need to be hosted on the site itself in the `assets` directory, preferably in a sensibly named subdirectory.

> ⚠️ Look to future-proofing your file naming/storage system; if it is likely that similar files will be continue to be uploaded for several years (i.e. talk slides), then consider adding a subsubdirectory indicating the year, or otherwise organising your file(s) in a sensible way.

To access your files in a post, you can use `../` to go up a level in a relative path (which you will need to do, as posts are in a separate directory). You must also wrap any paths/file names that include spaces with angle brackets:

```md
... to see my awesome file, click [here](<../assets/myfiles/my file name with spaces.md>).
```

Please also tag your posts with some or all of the following:

|     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- |
| Tag | <year>    |`events`                        | `updates`             | `talks`      | `sport` |
| For | all posts | socials, circles, competitions | elections, ball, WIMP | weekly talks | sport   |


