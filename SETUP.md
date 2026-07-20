# Create Your Own Mindspace

No coding experience required.

If you can upload photos to Facebook, you can build a Mindspace.

Mindspace gives you a customizable personal website for your thoughts, ideas, photos, videos, and creative work.

You will use GitHub to store the website and GitHub Pages to publish it for free.

---

# Before You Begin

You will need:

- A free GitHub account
- A short homepage video
- A few thoughts, quotes, or ideas
- About 15–30 minutes

You do not need to know how to code.

---

# Step 1: Create a GitHub Account

Go to:

https://github.com

Click:

**Sign Up**

Choose a username and create your account.

Think of GitHub as the place where your website files live.

Your username will also appear in your website address.

Example:

```text
https://yourusername.github.io/your-repository-name/
```

---

# Step 2: Create Your Own Copy of Mindspace

At the top of the Mindspace repository, click:

**Use this template**

Then click:

**Create a new repository**

Give your repository a name.

Examples:

```text
field-notes
late-night-thoughts
life-in-progress
my-mindspace
the-archive
```

Choose:

```text
Public
```

Then click:

**Create repository**

You now have your own copy of Mindspace.

---

# Step 3: Understand the Files

Your repository should include files similar to these:

```text
README.md
SETUP.md
config.js
index.html
thoughts.html
styles.css
hero.mp4
```

Each file has a different purpose.

The good news is that most users only need to edit two of them.

---

# What Do I Actually Need to Edit?

Most Mindspace users only need to customize:

```text
config.js
hero.mp4
```

That is where your personal content lives.

You should not need to edit the rest of the website code.

---

## config.js

This file controls:

- Your website title
- Your tagline
- Your homepage statement
- Your author name
- Your colors
- Your thoughts
- Your quotes
- Your homepage video filename

A typical section may look like this:

```javascript
const SITE = {
  title: "My Mindspace",

  tagline: "A public archive of private thinking.",

  statement: "This is not advice. It's evidence of thinking.",

  author: "@yourname",

  heroVideo: "hero.mp4",

  theme: {
    background: "#080808",
    text: "#F5F2EA",
    accent: "#D6FF2F",
    muted: "#9A9A9A"
  },

  thoughts: [
    {
      type: "thought",
      date: "July 2026",
      text: "Replace this thought with your own."
    }
  ]
};
```

You can change the words and colors without touching the rest of the website.

---

## hero.mp4

This is your homepage background video.

Replace the sample video with your own.

Ideas:

- Travel footage
- Camera roll memories
- Ocean footage
- City lights
- Coffee shop scenes
- Nature clips
- Creative projects
- Personal moments

Keep the video under 30 seconds when possible.

For better loading speed, try to keep the file under 20–30 MB.

The filename should stay exactly:

```text
hero.mp4
```

---

# Files You Do Not Need to Edit

Most users should not need to open:

```text
index.html
thoughts.html
styles.css
```

These files power the website behind the scenes.

Leave them alone unless you want to make advanced design or layout changes.

### index.html

Controls the homepage structure.

### thoughts.html

Controls the one-thought-per-screen archive.

### styles.css

Controls the visual design, layout, fonts, spacing, and animations.

You do not need to understand these files to use Mindspace.

---

# What Happens Automatically?

Once you customize:

```text
config.js
hero.mp4
```

Mindspace automatically creates the rest of the experience.

## Homepage Features

The homepage includes:

- A fullscreen hero video
- Automatic video playback
- Muted sound by default
- Infinite video looping
- A Sound On / Sound Off button
- Your website title
- Your tagline
- Your homepage statement
- An Enter the Archive button

The video starts automatically when someone visits your page.

Because most browsers block automatic sound, the video begins muted. Visitors can turn the sound on using the sound button.

---

## Archive Features

The thoughts page includes:

- One thought per screen
- Vertical scrolling
- Smooth scroll snapping
- Progress dots
- Keyboard navigation
- Mobile-friendly design
- Thought numbers
- Thought or quote labels
- Dates
- A link back to the homepage video

Your archive content is created automatically from the thoughts inside:

```text
config.js
```

You do not need to add thoughts directly to `thoughts.html`.

---

# Step 4: Replace the Homepage Video

Find:

```text
hero.mp4
```

Open the file menu and delete the sample video.

Confirm the deletion by clicking:

**Commit changes**

Then return to the main repository page.

Click:

```text
Add file
→ Upload files
```

Upload your own video.

Make sure the uploaded file is named:

```text
hero.mp4
```

Then click:

**Commit changes**

Your new homepage video is now stored in the repository.

---

# Step 5: Customize Your Website

Open:

```text
config.js
```

Click the pencil icon to edit the file.

---

## Change Your Website Title

Find:

```javascript
title: "My Mindspace"
```

Replace it with your own title.

Example:

```javascript
title: "Field Notes"
```

Other ideas:

```text
Late Night Thoughts
Life in Progress
The Archive
Fragments
Things I Don't Want to Forget
```

---

## Change Your Tagline

Find:

```javascript
tagline: "A public archive of private thinking."
```

Replace it with your own message.

Examples:

```javascript
tagline: "Things I don't want to forget."
```

```javascript
tagline: "Fragments from a life in progress."
```

```javascript
tagline: "Ideas, memories, and unfinished thoughts."
```

---

## Change Your Homepage Statement

Find:

```javascript
statement: "This is not advice. It's evidence of thinking."
```

Replace it with your own statement.

Examples:

```javascript
statement: "Strong opinions. Weak attachment."
```

```javascript
statement: "Ideas before they become respectable."
```

```javascript
statement: "Certainty is overrated."
```

---

## Change Your Name

Find:

```javascript
author: "@yourname"
```

Replace it with your name, username, or nickname.

Example:

```javascript
author: "@janedoe"
```

---

# Step 6: Add Your Thoughts and Quotes

In `config.js`, find:

```javascript
thoughts: [
```

Each entry should look like this:

```javascript
{
  type: "thought",
  date: "July 2026",
  text: "Replace this thought with your own."
}
```

Replace the sample text with your own.

Example:

```javascript
{
  type: "thought",
  date: "July 2026",
  text: "Most people are not afraid of failure. They are afraid of failing publicly."
}
```

---

## Add a Quote

Use:

```javascript
{
  type: "quote",
  date: "July 2026",
  text: "A strong opinion should still leave the door unlocked."
}
```

---

## Add More Entries

Place a comma after the previous entry, then add another one.

Example:

```javascript
thoughts: [
  {
    type: "thought",
    date: "July 2026",
    text: "Most people are not afraid of failure. They are afraid of failing publicly."
  },

  {
    type: "quote",
    date: "July 2026",
    text: "A strong opinion should still leave the door unlocked."
  },

  {
    type: "thought",
    date: "July 2026",
    text: "Ideas deserve a home, not just a timeline."
  }
]
```

Be careful not to remove:

- Quotation marks
- Commas
- Curly brackets
- Square brackets

When finished, click:

**Commit changes**

Your archive will update automatically.

---

# Step 7: Change the Colors

Inside `config.js`, find:

```javascript
theme: {
  background: "#080808",
  text: "#F5F2EA",
  accent: "#D6FF2F",
  muted: "#9A9A9A"
}
```

You can replace these color codes with your own.

### background

The main background color.

### text

The main text color.

### accent

The highlight color used for numbers, buttons, and details.

### muted

The softer text color used for dates and labels.

Example:

```javascript
theme: {
  background: "#10131A",
  text: "#F7F1E8",
  accent: "#FF6B6B",
  muted: "#8D93A1"
}
```

You can search online for:

```text
hex color picker
```

to find color codes you like.

---

# Step 8: Publish Your Website

Open your repository.

Click:

**Settings**

In the left menu, click:

**Pages**

Under:

```text
Build and deployment
```

Find:

```text
Source
```

Choose:

```text
Deploy from a branch
```

Under:

```text
Branch
```

Choose:

```text
main
```

Under the folder menu, choose:

```text
/ (root)
```

Click:

**Save**

GitHub will begin publishing your website.

---

# Step 9: Wait for GitHub to Build the Site

GitHub usually needs a few minutes to publish your page.

You can check the status by opening:

```text
Actions
```

Look for a workflow called:

```text
pages build and deployment
```

A green check means the website was published successfully.

A yellow circle means it is still working.

A red X means something went wrong.

---

# Step 10: Find Your Website Address

Return to:

```text
Settings
→ Pages
```

GitHub should show a message similar to:

```text
Your site is live at:
https://yourusername.github.io/your-repository-name/
```

For example:

```text
https://janedoe.github.io/field-notes/
```

That is your website.

Share it.

Bookmark it.

Make it yours.

---

# Updating Your Site Later

You do not need to republish the website manually every time.

GitHub Pages updates the site automatically whenever you save changes to the repository.

To add a new thought:

1. Open `config.js`
2. Click the pencil icon
3. Add the new thought
4. Click **Commit changes**
5. Wait a minute or two
6. Refresh your website

To replace the homepage video:

1. Delete the existing `hero.mp4`
2. Upload a new file named `hero.mp4`
3. Commit the change
4. Refresh the website after GitHub finishes updating it

---

# Important File Rules

Use these exact filenames:

```text
config.js
hero.mp4
index.html
thoughts.html
styles.css
```

GitHub filenames are case-sensitive.

That means:

```text
hero.mp4
```

is different from:

```text
Hero.mp4
```

Do not rename the files unless you also know how to update the website code.

---

# Troubleshooting

## My website is blank

Check that:

- `index.html` is in the main repository folder
- GitHub Pages is set to `main` and `/ (root)`
- Your files were committed
- The Pages deployment finished successfully

---

## My video does not appear

Check that:

- The file is named exactly `hero.mp4`
- The video is in the same folder as `index.html`
- The video uses MP4 format
- The video uses H.264 when possible
- The file is not extremely large

---

## My changes are not showing

Try:

1. Wait one or two minutes
2. Refresh the page
3. Use a private or incognito browser window
4. Check the GitHub Actions tab for deployment errors

---

## My thoughts are not appearing

Check your `config.js` file for missing:

- Commas
- Quotation marks
- Curly brackets
- Square brackets

Compare your entry to this format:

```javascript
{
  type: "thought",
  date: "July 2026",
  text: "Your thought goes here."
}
```

---

# See a Live Example

View Intellectually Questionable:

https://iqtheengineer.github.io/intellectually-questionable/

It demonstrates the type of personal, cinematic space you can create with Mindspace.

---

# You Built Your Own Website

No algorithm.

No feed.

No hosting bill.

Just your own corner of the internet.

Welcome to Mindspace.

## ⭐ Like the idea?

If Mindspace resonates with you, please give this repository a star.

Every star helps more people discover a simpler way to build their own corner of the internet.

Thank you for supporting the project.
