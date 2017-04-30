# Introduction

Methodological advances are the lifeblood of the historical profession and the most recent significant advancement in methods has been the application of digital techniques in research.  According to the American Historical Association, “only three positions even mentioned digital history back in 2003–04, and 10 positions made a similar request in 2008–09” but in 2012 32 positions or 4 percent of all positions advertised “mentioned digital skills” as a requirement or benefit for applying academics.   When contrasted with the slow and even declining growth of the historical profession over the past several years, one can clearly see the incentive for graduate students to learn this new methodology. Moreover, the advent of digital methods is not merely a buzzword to get new PhDs hired but it also, like any other methodology, presents an opportunity to ask new questions of old sources, or at the very least approach old queries in new ways.

With this context in mind, this project is a blend of the old and new methodological approaches.  In a past reading of Cicero’s *Pro Caelio Oratio* in English, I had noticed that in the translation of Cicero’s most famous speech, the author often paired mentions of Clodia with the passive voice and Caelius with the active. Likewise, Caelius seemed to be the subject of the sentence, appearing before the verb, while Clodia seemed more often than not to after the verb.  My curiosity was peaked as to whether or not this was merely a feature of the translation itself, or if this trend was actually part of Cicero’s invective. It seemed within the realm of possibility that he intentionally used the active and passive voice to support or impugn as part of his rhetoric.  This also seemed the perfect time to apply digital methodologies in order to gain a better understanding of the methods themselves, as well as see the extent to which such an approach could help my analyses.

# Historiography and Digital Influences



# Methodology and Digital Applications

In order to apply any kind of digital practice to an analysis of the *Pro Caelio*, the text first needed to be scraped off of a site using a non-copyrighted version of the text.  The Perseus collection seemed the most logical choice for this as it was already curated in a reasonably accessible format and used a non-copyrighted version of the *Pro Caelio*.  There were downsides in choosing to use Perseus’s archive, as it unfortunately uses older versions of most texts, but the upsides of accessibility and its status as a curated university database were worthy reasons to offset this weakness. Further, since I needed to obtain an uncopyrighted version of the oration, anything I would obtain would have to be relatively outdated as a text anyway, so this shortcoming was not as great as one might initially suppose. Finally, as this is mostly a proof-of-concept for measuring the zeitgeist of Cicero’s language more so than an extremely close textual analysis, the problem of the version’s age was largely mitigated.

So that others can easily test and apply my methodology, I will be explicit in recounting it. Using the freeware, *Web Scraper* in Google’s *Chrome* browser, one can scrape the text off Perseus’s website, first by identifying the text they would like to scrape on the page and adding it as a selector, then by identifying the links that the scraper would cycle through as an additional selector. One then simply needs to make a copy of the text selector and place it within the branch of the link selector. The *Web Scraper* can then be activated and it will scrape the text.

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture1.jpg)

Next, the scraped information needed to be scrubbed to make the text searchable before finally placing the text in a program that allowed for easy searching within the document.  If this process were not completed, it would lead to the search missing names and suffixes for verb endings, so this step is essential to the process.  I was in luck that the still in development *Arakhne* program was available for my use, and although it currently lacks some advanced features that its curator plans to implement in the future, it is nonetheless a stellar Latin text scrubber.  Unfortunately, *Arakhne* is not yet ready to run on Windows machines, but luckily custom-created environments exist to circumvent this.  For this purpose, I used *DHbox*, a tool created expressly for digital humanities research to act as a platform within which *Arakhne* could run.

Two functions within *Arakhne* that are of great aid to textual analysis are its scrubbing and lemmatizing features.  The scrubbing feature, as previously mentioned, allows for an easy scanning of the text. By copying the code intended for this use, *Arakhne* scrubbed the program.

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture2.jpg)

After scrubbing, the processed text was copied from a .csv file into a Microsoft *Word* document.

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture3.jpg)

The lemmatizing feature is equally impressive and important as it morphs the words from their various forms into uniform cases and declensions, so that specific words can easily be located through any search feature. The lemmatized version, for sake of comparison, is shown below.

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture5.jpg)

Although the aims of this project reduced the utility of the lemmatized version, it was particularly important to obtain an accurate count of each name that was included in the final analysis. Because case endings for names vary in Latin as much as any other noun, it would be difficult to obtain an accurate count to make certain that the search feature found every iteration of each name. The lemmatized text largely eliminates this problem, since each name is reset to a single ending, making it easily searchable.

After obtaining the proper count for each name in the lemmatized text, I turned towards the actual text analysis.  Each name and passive verb ending was marked via the find feature in *Word*. An example of this process is shown below.

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture6.jpg)

When searching for passive verb endings, the “match suffix” feature was utilized for the find feature to locate only verb endings and not combinations of letters that might appear earlier in words.  The result of highlighting different names and endings can be seen below.

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture7.jpg)

An immediate limitation in the find feature was that there was no realistic way around fourth principal part, passive verbs, as *sum* has too many irregularities and uses in Latin grammar to be useful in identifying these verbs and the endings in the verbs themselves are too typical as noun endings. This unfortunately required that I read the context around each name to identify these verbs.  While the matter was made much easier than it would have otherwise been in reading the text without name and ending highlighting, it shows that there is still much work to be done to make textual analysis of grammar completely streamlined.

# Findings

The final tally noting the juxtaposition of passive-active verbs and the function of prosecutor’s and defender’s names as subjects (or subject-modifying) or objects (or object-modifying) in Cicero’s syntax can be seen in the table below.   It should be noted that since the aim of this work was to use the text search functions to their utmost, Cicero’s references to these characters without explicit mention of their names were not included in the final tally.

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture8.jpg)

While the above note is an enormous caveat, that would be the work of a much larger project, perhaps one that also included a more detailed analysis of the context in which these dynamics ensued.  Still, there are some cases from this sample that are worth mentioning.  Explicit mentions of Clodia and Atratinius are only mentioned as objects. The only exception to this rule is when Clodia’s name appears with Caelius.  This placement as an object might have enhanced Cicero’s invective.  While this is a curious phenomenon, without a deeper look at when Clodia is referenced as a pronoun rather than by name, this trend remains inconclusive due to sample size.  This assumption also seems more doubtful when one notes that Caelius’ name often appears as an object.

Overall, rather than revealing as much about Cicero’s use of the active and passive voice in his invective, these numbers more depict...
