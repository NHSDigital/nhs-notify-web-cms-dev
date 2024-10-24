---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Letter templates
parent: Using NHS Notify
nav_order: 4
permalink: /using-nhs-notify/letter-templates
section: Writing a message
---

Upload a Word document of a letter and NHS Notify will print and post it for you.

## How to edit your letter using our template

Your Word document must meet our letter specification. The page size and layout is A4 portrait (210 x 297mm).

Download the relevant letter template to set up your letter:

- [letter template]({% link assets/worddocs/letter-template-nhs-notify.docx %})
- [large print letter template]({% link assets/worddocs/letter-template-nhs-notify-large-print.docx %})
- [other language letter template]({% link assets/worddocs/letter-template-nhs-notify-other-language.docx %})
- [other language letter (right aligned)]({% link assets/worddocs/letter-template-nhs-notify-other-language-right-aligned.docx %})
- [parent or guardian letter template]({% link assets/worddocs/letter-template-nhs-notify-parent-or-guardian.docx %})

You can save the template and edit it with your message content.

## Formatting your letter

Do not edit the page margins in the letter template. It has the correct formatting and layout for printing.

Organise your message content using the styles in the template.

If you’re copying and pasting text from another document, paste it without any formatting. Then [apply the styles](https://support.microsoft.com/en-gb/office/apply-styles-f8b96097-4d25-4fac-8200-6139c8093109) in the template.

You can also use [Microsoft Word’s format painter](https://support.microsoft.com/en-gb/office/use-the-format-painter-4bb415a9-d4e4-42b7-b579-170adc594e40) to copy the formatting of the styles and apply it to your text.

Find out how to use:

- [personalisation](#personalisation)<!-- markdownlint-disable-line -->
- [font and font size](#font-and-font-size)
- [headings](#headings)
- [paragraphs and body text](#paragraphs-and-body-text)
- [links](#links)
- [bullet points](#bullet-points)
- [images](#images)
- [QR codes](#qr-codes)

You can also find out about content you should not edit, including the:

- [address field](#address-field)
- [NHS logo](#nhs-logo)
- [NHS number](#nhs-number)
- [date](#date)
- [page count](#page-count)

## Personalisation

To add a personalisation field, include a placeholder with double brackets around it. For example:

{% include components/inset-text.html
    text='Hello ((firstName)), your NHS Number is ((nhsNumber))'
%}

Read about the [personalisation fields]({% link pages/using-nhs-notify/personalisation.md %}) that are available in the Personal Demographics Service (PDS) and how to provide your own personalisation data.

## Font and font size

The font size for standard letters is 12 points. The font size for large print is 16 points.

NHS Notify prints letters in the font Noto Sans.

### Downloading your font

Noto Sans is a free font.

Download Noto Sans to ensure that you can edit and view your template as it will be printed.

1. Go to [Noto Sans on Google Fonts](https://fonts.google.com/noto/specimen/Noto+Sans). Select 'Download all' to download Noto Sans to your device as a zip file.
2. Right click the zip file and select 'Extract all'.
3. Open the file. Right click 'NotoSans-Italic-VariableFont_wdth,wght' and select 'Install'. Right click 'NotoSans-VariableFont_wdth,wght' and select 'Install'.
4. Open the folder 'static'.
5. Select all of the files in this folder by dragging your mouse over them or selecting 'ctrl' + 'a' on your keyboard. Right click and select 'Install'.

Noto Sans will now be available in Microsoft Word.

## Headings

Use the style ‘Heading 2, NHS letter heading' in the template for headings.

Headings are in bold. They are not in italics or underlined.

Use the main heading to summarise what your letter is about.

Use headings to break your content up and to help recipients find what they need.

## Paragraphs and body text

Use the style 'Normal' in the template for body text.

Paragraphs can be split across 2 pages.

If you do not want a paragraph to run over different pages, add a page break before the paragraph.

## Links

Use the style ‘Hyperlink' in the template for links.

Write links in full, starting with https://. For example:

{% include components/inset-text.html
    text='<b><span>https://www.service-manual.nhs.uk/content</span></b>'
%}

Links in letters are in bold to make them stand out. Do not use underlined text or italics.

Do not split links across different pages. Add a page break before the paragraph with the link if needed.

### Short URLs

If you have a long, complex web address, you can [request a short URL from GOV.UK](https://www.gov.uk/guidance/contact-the-government-digital-service/request-a-thing#short-url). This can take some time and may delay your template creation.

We do not recommend using a third-party link shortening service because:

- your users cannot see where the link will take them
- your link might stop working if there’s a service outage
- you can no longer control where the redirect goes

## Bullet points

Use the style 'List paragraph' in the template for bullet points.

You can use bullet points to make your text easier to read. Make sure that:

- you use a lead-in line
- the bullets make sense running on from the lead-in line
- you use lower case at the start of the bullet
- there are no commas, full stops or semicolons at the end of bullets

## Images

Images must be black and white. Position them within the same page margins as the text.

## QR codes

If you want to include a QR code, put it in the body of your letter. Insert it as an image.

You’ll need to generate the QR code yourself.

You must also provide a short URL or written instructions for how to find your webpage. For example:

{% include components/inset-text.html
    text='<span>scan the QR code or visit <b>https://www.notify.nhs.uk</b></span>'
%}

## Content you should not edit

### Address field

The address field fits inside the address window on the envelope.

The address is a personalisation field and is set automatically.

The recipient’s name is always included as the first line of the address. For a letter about a child, the first line will include 'Parent or guardian of'.

### NHS logo

The NHS logo is black and white. It's positioned in the top right of the letter.

### NHS number

The recipient's NHS number appears above the body content of the letter and is right aligned.

It's a personalisation field and is set automatically.

### Date

The date that will be printed is the date when the letter is dispatched. It's set automatically.

It appears above the body content of the letter and is right aligned.

### Page count

The page count shows the current page number and the total number of pages. For example:

{% include components/inset-text.html
    text='Page 1 of 2'
%}

It updates automatically.