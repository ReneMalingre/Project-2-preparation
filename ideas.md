## Project Two - Ideas

## 💡Idea: Contact Lens Parameter Database (enter spec Rx, give options based on Rx etc)

### User: Optometrist

There are about 100 disposable contact lens types on the market. They vary in fitting parameters to suit differently shaped eyes, and cover different lens power ranges. They are made from a wide variety of materials to suit different needs and physiologies, and they vary in how many times they can be worn before replacement. The same lens may come in multiple pack sizes. It is very hard to keep all of this in your head, and there is no online tool that allows you to search for the ideal lens to suit your patients.

#### ✅Proposal

Create a database and its front-end that allows all of these parameters can be entered into

Allow searching for power, or nearest power match based on adjustable criteria, material type, shape, etc, etc

A good, real-world, monetizable app with only limited (paper!) competition

## 💡Idea: Spectacle product information (frame, lenses, warranty)

### User: Optometrist/Optical Retailer

Every pair of spectacles is different, and frames and especially spectacle lenses contain a lot of technology that gives them features and benefits that the consumer is not fully aware of. This sometimes leads them to believe that spectacles are expensive, because they are not aware of the value to them they contain.

#### ✅Proposal

Based on the spectacle frame and lens chosen, the consumer can log in to a website and view a page made from templates that gives them information about the frame brand story, its manufacturing, warranty and care instructions, and information about the lens manufacturer story, lens family features technology and benefits, and the features and benefits of the lens material, tint features and surface coatings, warranty and care instructions.

A good, real-world, monetizable app with no competition

## 💡Idea: Check details Questionnaire (prefilled web form)

### User: Health Clinic, Personal Services Clinic

A key part of looking after patients in a health setting is accurate personal information so that appropriate care can be given and privacy maintained. A part of this is to check patients name, address, date of birth, care giver details, their other health practitioners, communication preferences and permissions and relevant lifestyle and health information. No-one likes to fill in forms, and they particularly don't like entering information that they feel the survey-giver should already know.

#### ✅Proposal

Give a web-based, prefilled survey that allows the patient to confirm, change or add new information, prefilled with existing information for that patient, exported from whatever system the practitioner uses in either XML or JSON format, imported into our system to seed the questionnaire, and when completed, re-exported for reimporting to the practice management system.

Two modes, front desk where the staff selects the patient so the patient receives, say, a tablet with the survey, or the patient is given a unique code via text or email that allows them to log in.

The key difference here is that it is platform-independent and I haven't found a system that pre-loads the known information to save the hassles.

## 💡Idea: Informational report generator

### User: Health Clinic/Consultant/Many businesses

40-80% of advice given to patients is forgotten immediately. Information in written form helps to clarify and reinforce important messages and advice and instructions. Paper leaflets are sometimes provided, but it is a burden to keep these up-to-date and printed in the appropriate quanity to ensure they are on hand and that money is not wasted on printing. There can be a reluctance to give them out if the patient or customer believes they can remember what was said, in a normal over-estimation of their own ability to recall information.

#### ✅Proposal

Using a web-based form to select from a list of pre-written information templates, with the option to add custom information, will generate a HTML page dynamically that can either be viewed online through a login or sent via an HTML email directly to the patient.

- Eg: You are myopic – here are some facts
- Everything is fine: see you in two years unless you have problems
- Here is how to clean your eyelash line to avoid infection and improve your dry-eye
- Thanks for visiting: here is some information about your visit and your practitioner, and when you should return.
- Suggest use markdown and use an npm package to convert it to html