# use-all-polly-voices-with-lang-tag
Will show you how to use all available Amazon Polly voices for your specific language/country. This will help you to create 50+ personas with unique voices for your immersive Alexa skills.

# Background
Amazon announced the public availability of Amazon Polly voices for Alexa skills in October 2018 (1). There are currently 58 Polly voices available (2). 

The Polly voices can be used within any SSML speak text for speakOutput as well as reprompt: 

`<voice name="Brian">Hello, this is Brian speaking. How are you doing today?</voice>`

See? Pretty easy to use!

But some languages only have one or two voices. I needed a few more individual voices for an Alexa skill I wrote. So I was looking for a way around the limitation.

# Solution

In order to create more personas for your skill with an individual voice, you can use all the Polly voices available worldwide. It's easy, because there is something called...

... the <lang> tag (3)! The <lang> tag can be used within an SSML to make sure Alexa is using a language specific pronunciation. But this can also be used to let other Polly voices speak another language, with an accent (4). For example you can use a French Polly voice to talk American English with a Frech accent. How? I will show you.
  
`<voice name="Celine"><lang xml:lang="en-US">Hi, my name is Celine. Nice to meet you, Brian. How are your doing, Brian?</lang></voice>`

Easy as that. Now, get back your skill and use Polly voices. Check out my other repo to see how to use polly voices with background music! It's also pretty easy!

  
  (1): https://developer.amazon.com/blogs/alexa/post/baee53c1-5b03-4580-b57a-ee9510413354/amazon-polly-voices-in-alexa-skills-now-generally-available
  
  (2): https://docs.aws.amazon.com/en_us/polly/latest/dg/voicelist.html
  
  (3): https://developer.amazon.com/docs/custom-skills/speech-synthesis-markup-language-ssml-reference.html#lang
  
  (4): https://docs.aws.amazon.com/en_us/polly/latest/dg/supported-ssml.html#lang-tag
