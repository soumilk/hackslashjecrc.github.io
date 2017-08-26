# hackslash.org/
#### This is the source for the HackSlash website, powered by [Jekyll](https://jekyllrb.com/)

[![Build Status](https://travis-ci.org/hackslashjecrc/hackslashjecrc.github.io.svg?branch=master)](https://travis-ci.org/hackslashjecrc/hackslashjecrc.github.io)

Feel free to suggest changes to our website.

### Setup
- Please ensure [**Ruby**](https://www.ruby-lang.org/en/documentation/installation/) is installed
    * Use ```ruby --version```, to verify if ruby is installed.
    * Also make sure ```bundler``` is installed by ```sudo gem install bundler```
- Install ```jekyll``` using ```sudo gem install jekyll```
- ```git clone https://github.com/hackslashjecrc/hackslashjecrc.github.io```
- ```cd hackslashjecrc.github.io```
- ```jekyll serve``` or ```jekyll build```

### Contributing to the website
To keep layout and design same throughtout the website, use _layout_ - ```default``` and for team members profile use ```people``` layout.
#### For pages
```yml
---
layout: default
title: PageName - HackSlash
description: PageName - HackSlash
id: category
---
```

#### Team Members
- The profile page should be in ```people/``` dir, and name as _username.html_
```yml
---
layout: people
title: Name | Team - HackSlash
description: Name | Team - HackSlash
id: team
person: Name
designation: Team Member
branch: Branch
img: image #/assets/people/
email: email
facebook: username
twitter: username
github: username
linkedin: username
skills:
  - skill: Skill 1
  - skill: Skill 2
bio: A bio about yourself
---
```
- The team directory list
Mention details in ```_data/team.yml``` file
```yml
- id: username //the same as above created file
  name: Full Name
  img: image name #/assets/people/
  branch: Branch
  role: Team Member
  skills: Skills
```
- The image
The image should be placed in ```/assets/people/``` folder with the same name specified in ```team.yml``` data file and ```/people/name.html``` file.
Recommended size of image - _480x480_
