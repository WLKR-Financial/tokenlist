# 🔍&nbsp;&nbsp;WLKR-Uniswap Token List

Not sure how to submit a pull request with the changes outlined below? Use our Customisation Request form for a hands off approach.

**[Request Form (Coming Soon)](https://docs.google.com/forms)**

## 🕵️&nbsp;&nbsp;Custom Index Details v0.1

In order to add your own details for your Index, and verify it, please follow these steps:

1. Get started by forking this repository
2. Add a new file into the `set-details` folder that is named: `[insert-your-set-address].setdetails.json` (i.e. 0x1494CA1F11D487c2bBe4543E90080AeBa4BA3C2b.setdetails.json). A template can be found at `set-details/template.setdetails.json`
4. Be sure to include any required media such as token or manager icons in the `/assets` directory under their respective folders
5. Verify that the details match the required schema [here](https://github.com/WLKR-Financial/tokenlist/blob/main/set-details.schema.json) by pasting the entire entry into this [schema validator](https://www.jsonschemavalidator.net) and see if your input JSON matches properly. See below if you need multi line descriptions
6. Create a pull request against the master branch and follow the pull request template to submit the proper signature (signed current version number [i.e. 1] via TokenSets UI)
7. Join our [Discord](https://discord.gg/wlkrfinancial) and ping a team member to review your submission  

#### 🦄&nbsp;&nbsp; TokenList Details
To add your Index details to our Tokenlist, or an Indexed Token not previously added, add an entry to the details in the `set.tokenlist.json` file, follow other submissions

#### 🛂&nbsp;&nbsp;Generating a Valid Signature
Each pull request must be accompanied by a valid signature signing the next monotomically increasing version number. To generate a signature:
1. Head over to your Index page on WLKRIndex `walkrfinancial.com/v2/set/your_set_address`
2. Once logged in, the name of your Set should appear in blue with an edit icon
3. Tap on your Set's name and follow the steps in the popup

#### 📰&nbsp;&nbsp;Multi Line Descriptions
If you need to have multi-line JSON, you can use a HJSON converter to help with writing it.

1. Head over to this [tool](https://hjson.github.io/try.html)
2. On the left pannel, paste your multi line description under the `multiline string` comment, replacing the JSON Haiku
3. Copy the output from the right pannel under `haiku`, omitting the trailing comma and paste into your `setdetails.json` file.
