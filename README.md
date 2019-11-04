# mailtemplates-made-easy
Using TiddlyWiki to create Mailtemplates

Description below is taken from the "How to use" tiddler you can view after downloading the TiddlyWiki.

## Setup

1. Create a mailtemplate like Mailtemplate:Request for Offer (see also below for syntax)
1. Create a form tiddler like Request for Offer

## Usage

1. Fill the form (Request for Offer)
1. Click the [create mail] button.
1. A new mail window will pop up. Check its content.
1. Send the mail

## Syntax Mailtemplate

* At the top of the template you need to define placeholders like  this: `[[`placeholder`:`Description`]]`.
* Each line may contain only one placeholder.
* The first empty line finishes the placeholder definition.
* After the first empty line, the mailtext follows.
* Use the placeholders in the form of `{{!!`placeholder`}}`.

### Special placeholders

These placeholders have to be defined:

1. `[[recipients:`list of mail recipients`]]`
1. `[[subject:`mail subject. May use placeholders in the form described above`]]`

#### Checkboxes

A placeholder ending with `_cb` defines a checkbox. It has to be followed by the values for the unchecked and the checked status.

`[[known_cb,`unchecked`,`checked`:`description`]]`

#### Dates

A placeholder ending with `_date` will generate a date-field.
