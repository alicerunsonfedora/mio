---
title: Frequently asked questions
---
# Frequently asked questions

## How do I create a mod in the first place?!
This FAQ will hopefully answer a few or all of your questions concerning modding.

## Which version of Ren’Py do I use?
While it is possible to test and write with the latest Ren’Py SDK, you’ll need version 6.99.12.4 of the SDK to properly compile it so it works with the DDLC binaries. It’s recommended to use this version for creation, testing and deployment of any DDLC mod.

<p><a href = "https://renpy.org/release/6.99.12" class = "p-button--positive p-link--external">Get the Ren'Py SDK</a></p>

## Can somebody help me with assets?!
It depends on what assets you need.

- Art: Most likely not, unless it is an easy edit or simple reposing.
- Music: This one is a possibility, but still unlikely.
- Poetry: This one is a lot more common due to people having more time to write than the previous two.
- Coding: Yes, but please have specific and direct questions to ask. We want to help, but you need to provide the question first.

## Are there any example mods I can look at for reference?
There are a few mods in the DDLC modding community that are indeed open-source, meaning that you can edit, inspect, and redistribute its code. Here are a few examples:

- [Doki Doki Endless Adventure](https://github.com/Sayo-nika/koizumi) (Sayonika Team)
- [Doki Doki: The Angel Returns](https://github.com/TheAngelReturns/the-angel-returns) (Project Alice)
- [Monika After Story](https://github.com/Monika-After-Story/MonikaModDev) (Monika After Story Team)

## How can I get characters to a spot?
You’ll need to make use of the transform property. The transform property is what tells Ren’Py where the character goes on the screen and if they’re in focus or now. There are a few things you need to know about your particular scene:

- How many people are involved?
- What order should they be in?
- Who’s in focus? Sinking?

The basic structure of the transform property looks like this.
<center><p class = "p-heading--three">t32</p></center>

Where the following apply:

- ‘t’ determines if the character is in focus or sinking. There are four possibilities:
    - ‘t’ - Not in focus, but there
    - ‘f’ - In focus (usually enlarged for effect)
    - ‘s’ - sinking
    - ‘l’ - appears from the left of the screen
- The first number determines how many people are present. The maximum is four and the minimum is one.
- The second number determines where they are placed. To make it easier, you can ask “is this person the nth person in the line?”.

## My characters are huge! What am I doing wrong?
It’s highly possible that you forgot to add the transform property to them. These are usually defined by the `at` command. See “How can I get the characters to a spot?” for more details. Also, you may have made your asset too big or didn’t make the correct sizing.

## Why do I seem to not be making any progress?
Most likely you are, anything you do to create a mod is worthwhile in the end. Such as adding the definitions, or even just adding a custom face edit.

## I need a particular asset. How can I make a request?
The DDMC community is more than willing to assist you depending on what you need. Here are some tips to ensure your request is heard and valid:

- Check the content channels first. You may never know if the asset you’re looking for has already been posted.
- Place your request in #content_requests. This is for organization’s sake.
- Ping your respective group once, but not more. People assigned to that role are aware of your request, but they may be busy.
- Describe exactly what you need in your request. Community members/assistants shouldn’t have to guess what you need; they are human, after all.
- Remember to respect the human in your request. Refrain from using demanding statements or using a certain type of language that would off-put the reader.

## Where can I get the original scripts?
There are multiple ways to fetch said scripts, but the most accessible way is through the Monika After Story team’s GitHub repository. They provide the story scripts online; any other scripts are located in the DDLC Mod template.

<p><a href = "https://github.com/Monika-After-Story/DDLCModTemplate/tree/master/original_story_scripts" class = "p-button--positive p-link--external">Get the original scripts</a></p>
