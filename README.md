# Business Card Template using `fastn`

This repository provides a prototype to create customizable business card 
design using the `fastn` language. You can create designs which can be used 
by users to easily create professional business card by filling in their 
information.

[![Watch the video](https://img.youtube.com/vi/Rys5CI9KQsg/hqdefault.jpg)](https://youtu.be/Rys5CI9KQsg)


## Getting Started

To use this template, follow the steps below:

1. Click on `Use this Template` or go to the following [link](https://github.com/new?template_name=repo_name&template_owner=fastn-community)
2. Enter the required details to create new repository (**Note**: repository name should be in kebab case).
3. Clone this newly created repository to your local machine.
4. Open the `fastn` file named `index.ftd` in a text editor.

## Creating a new Business Card category

The `index.ftd` file contains placeholders that you can replace with your own information. Here's what you need to do:

### 1. Replace Package Information

In the section labeled "DOCUMENTATION FOR YOUR CARD COMPONENTS", locate the 
`docs.home-card` component and check the following placeholders:

**Note:** All these are auto-filled values during repository creation

- `package-name`: Your repository name
- `package-full-name`: Your GitHub repository's full URL
- `license-url`: URL to the license of your choice (e.g., MIT License) (This 
  is currently commented, you can uncomment it if you want to include license.)
- `github`: Your GitHub Repository URL

### 2. Implement Front and Back Components

In the "DEFINE YOUR CARD COMPONENTS" section, you will find placeholders for implementing the front and back components of your business card.

For the both `front` and `back` component, you need to use the following 
headers (card details):

**Note:** These headers will be used by the users for filling in their 
information. It's mandatory to use all these headers while creating your 
component.

- `caption name`: You name (e.g., "John Doe")
- `string title`: Your job title
- `string company-name`: Your company name
- `ftd.image-src logo`: Image asset or Image URL to your company logo
- `optional string contact-1`: Your primary contact number (Optional for user)
- `optional string contact-2`: Your secondary contact number (Optional for user)
- `optional string email`: Your email (Optional for user)
- `optional string website`: Your email or social media link (Optional for user)
- `optional string address`: Your address (Optional for user)
- `optional string company-slogan`: A slogan or tagline for your company 
  (Optional for user)

If you want to create a **portrait** mode business card design, you can 
uncomment the `landscape: false` (line number: 39) in `lib.display-card` 
component invocation in `index.ftd` file

Replace the code present in the line numbers 47 to 52 with actual card's 
`front` side component implementation/definition.
Similarly, replace the code present in the line numbers 66 to 71 with actual 
card's `back` side component implementation/definition.

**Note:** It is **recommended** to create a `component/front.ftd` and 
`component/back.ftd` files for implementing `front` side and `back` side 
components respectively.

Also, `assets` for your package is auto-imported, you can use `assets` to 
add image etc. (Checkout `FASTN.ftd` file).

## Fix the README.md content

Replace the preview image with your template image 

- For `front` side: In [`.github/assets/front.png`](.github/assets/front.png)
- For `back` side: In [`.github/assets/back.png`](.github/assets/back.png) 


## Publishing your category design on Github page:

Check out [Publishing Static Site On github 
pages](https://fastn.com/github-pages/) to know more. 

Also add the live site link in **About** section of github repository.


## Some other information:

The sitemap present in `FASTN.ftd` is used to organise your package. 
This uses 

- `index.ftd`: It is the homepage which shows preview of front and back for 
  your card
- `how-to-use.ftd`: It is page that gives the detail descriptions about each 
  fields in the card component and how to use your package. It also shows 
  some variant of this card (like when some fields are present).

The documentation for this template comes from [`business-card`](fastn-community.github.io/business-card)


*To know more about `fastn`, visit [`fastn` website](https://fastn.com/). Also 
you can join our [discord](https://fastn.com/discord/) channel to connect 
with our team for further guidance.*
