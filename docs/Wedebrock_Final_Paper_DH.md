# Textual Analysis: Cicero's Use of Voice and Subject-Object Dynamics in his *Pro Caelio Oratio*

## Introduction

Methodological advances are the lifeblood of the historical profession and the most recent significant advancement in methods has been the application of digital techniques in research.  According to the American Historical Association, “only three positions even mentioned digital history back in 2003–04, and 10 positions made a similar request in 2008–09” but in 2012 32 positions or 4 percent of all positions advertised “mentioned digital skills” as a requirement or benefit for applying academics (Townsend 2013).   When contrasted with the slow and even declining growth of the historical profession over the past several years, one can clearly see the incentive for graduate students to learn this new methodology. Moreover, the advent of digital methods is not merely a buzzword to get new PhDs hired but it also, like any other methodology, presents an opportunity to ask new questions of old sources, or at the very least approach old queries in new ways.

With this context in mind, this project is a blend of the old and new methodological approaches.  In a past reading of Cicero’s *Pro Caelio Oratio* in English, I had noticed that in the translation of Cicero’s most famous speech, the author often paired mentions of Clodia with the passive voice and Caelius with the active. Likewise, Caelius seemed to be the subject of the sentence, appearing before the verb, while Clodia seemed more often than not to after the verb.  My curiosity was peaked as to whether or not this was merely a feature of the translation itself, or if this trend was actually part of Cicero’s invective. It seemed within the realm of possibility that he intentionally used the active and passive voice to support or impugn as part of his rhetoric.  This also seemed the perfect time to apply digital methodologies in order to gain a better understanding of the methods themselves, as well as see the extent to which such an approach could help my analyses.

The scope of this project is restricted by both the digital tools available and intentionally placed limitations.  Since it acts as a proof-of-concept for the application of digital technologies and methods towards linguistic analysis, my research question is two-pronged towards those ends. Ultimately, the goal was to define the benefits of limitations of technology-aided linguistic analysis using Cicero’s use of voice and subject-object structure as a case-study.  This project relied primarily on these digital technologies with my own skills in Latin used more for the evaluation of the program’s application than actual text analysis, although limitations in current technologies did require me to do some of the work manually. Still, the preliminary findings will show that the use of digital methods greatly increases the speed at which a textual analysis can be conducted.

# Historiography and Digital Influences

Text-based projects formed the basis for some of the earliest projects that utilized digital methodologies. At first, digitizing endangered texts were the focus of scholars’ and archivists’ efforts, preserving works that would be lost either due to the last copy’s fragile condition, or from their location in geo-politically unstable regions (Patrik 2007).  As the field increased in size, the application of digital tools expanded into analyses of the texts themselves.  As a result, the precedent for my own research into invective has already been set by other projects, such as one launched by the University of Chicago that examined the invective of American and non-American playwrights in black drama through a combination of text mining and machine learning (Argamon et al. 2009).   This growth in the discipline reflects the increasing size and importance of digital methods in mainstream, scholarly history, in the face of such momentous works my hope in inserting myself into the discipline is merely to reinforce the idea that these emerging methods can help even in smaller doses to make traditional linguistic analyses more achievable at the individual level.

On the historiographical side, no biographical or philological subject has been studied as often and deeply as Cicero.  This popularity is in part due to the unusual survival of much of his work from antiquity to the present day, but also because of his keen focus on Latin oratory and writing itself.  This proliferation of his writings was in large part due to the popularity of his works in antiquity, with even early Christian leaders such as Augustine citing him as a source of inspiration 300 years later (Augustine Confessiones 3.4; Tauris 2014, 249).  Modern historians have focused every facet of his life and work, from his life and influence, to his rhetorical style, to his grammar (Tauris 2014; Albrecht 2003; Cerutti 1999).  Because of the duality of historical and classical studies, the methodologies of studying Cicero have not evolved in a linear manner. Instead each discipline has incorporated methods of the other to varying degrees at different stages.  A clear example of this kind of methodological interchange is Anne Leen's "Clodia Oppugnatrix: The Domus Motif in Cicero's *Pro Caelio*," where Leen uses analytical frameworks from gender and cultural history in conjunction with a close reading and textual analysis (Leen 2000, 141-142). My contribution to the historiography follows a similar line, for while my focus is on Cicero's use of voice itself, the results speak towards whether or not voice, gender, and syntax have a relationship in his rhetoric.  The added digital component of my work also shows in part how the field progresses in its incorporation of new means of study.


# Methodology and Digital Applications

In order to apply any kind of digital practice to an analysis of the *Pro Caelio*, the text first needed to be scraped off of a site using a non-copyrighted version of the text.  The Perseus collection seemed the most logical choice for this as it was already curated in a reasonably accessible format and used a non-copyrighted version of the *Pro Caelio*.  There were downsides in choosing to use Perseus’s archive, as it unfortunately uses older versions of most texts, but the upsides of accessibility and its status as a curated university database were worthy reasons to offset this weakness. Further, since I needed to obtain an uncopyrighted version of the oration, anything I would obtain would have to be relatively outdated as a text anyway, so this shortcoming was not as great as one might initially suppose. Finally, as this is mostly a proof-of-concept for measuring the zeitgeist of Cicero’s language more so than an extremely close textual analysis, the problem of the version’s age was largely mitigated.

So that others can easily test and apply my methodology, I will be explicit in recounting it. Using the freeware, *Web Scraper* in Google’s *Chrome* browser, one can scrape the text off Perseus’s website, first by identifying the text they would like to scrape on the page and adding it as a selector, then by identifying the links that the scraper would cycle through as an additional selector. One then simply needs to make a copy of the text selector and place it within the branch of the link selector. The *Web Scraper* can then be activated and it will scrape the text.

---

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture1.jpg)

---

Next, the scraped information needed to be scrubbed to make the text searchable before finally placing the text in a program that allowed for easy searching within the document.  If this process were not completed, it would lead to the search missing names and suffixes for verb endings, so this step is essential to the process.  I was in luck that the still in development *Arakhne* program was available for my use, and although it currently lacks some advanced features that its curator plans to implement in the future, it is nonetheless a stellar Latin text scrubber.  Unfortunately, *Arakhne* is not yet ready to run on Windows machines, but luckily custom-created environments exist to circumvent this.  For this purpose, I used *DHbox*, a tool created expressly for digital humanities research to act as a platform within which *Arakhne* could run.

Two functions within *Arakhne* that are of great aid to textual analysis are its scrubbing and lemmatizing features.  The scrubbing feature, as previously mentioned, allows for an easy scanning of the text. By copying the code intended for this use, *Arakhne* scrubbed the program.

---

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture2.jpg)

---

After scrubbing, the processed text was copied from a .csv file into a Microsoft *Word* document.

---

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture3.jpg)

---

The lemmatizing feature is equally impressive and important as it morphs the words from their various forms into uniform cases and declensions, so that specific words can easily be located through any search feature. The lemmatized version, for sake of comparison, is shown below.

---

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture5.jpg)

---

Although the aims of this project reduced the utility of the lemmatized version, it was particularly important to obtain an accurate count of each name that was included in the final analysis. Because case endings for names vary in Latin as much as any other noun, it would be difficult to obtain an accurate count to make certain that the search feature found every iteration of each name. The lemmatized text largely eliminates this problem, since each name is reset to a single ending, making it easily searchable. The exception cases occurred when some names were not recognized within the word list that Arakhne operates on. Fortunately, there were only a few that went unrecognized and this problem was solved by searching for the beginning of each person’s name and individually filtering out undesired findings. As an example, for Herennius’s name in the text the search “Herren” was used, which netted two search results, both of which referred to Herennius and not another noun.

After obtaining the proper count for each name in the lemmatized text, I turned towards the actual text analysis.  Each name and passive verb ending was marked via the find feature in *Word*. An example of this process is shown below.

---

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture6.jpg)

---

When searching for passive verb endings, the “match suffix” feature was utilized for the find feature to locate only verb endings and not combinations of letters that might appear earlier in words.  The result of highlighting different names and endings can be seen below.

---

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture7.jpg)

---

An immediate limitation in the find feature was that there was no realistic way around fourth principal part, passive verbs, as *sum* has too many irregularities and uses in Latin grammar to be useful in identifying these verbs and the endings in the verbs themselves are too typical as noun endings. This unfortunately required that I read the context around each name to identify these verbs.  While the matter was made much easier than it would have otherwise been in reading the text without name and ending highlighting, it shows that there is still much work to be done to make textual analysis of grammar completely streamlined.

# Findings

The final tally noting the juxtaposition of passive-active verbs and the function of prosecutor’s and defender’s names as subjects (or subject-modifying) or objects (or object-modifying) in Cicero’s syntax can be seen in the table below.   It should be noted that since the aim of this work was to use the text search functions to their utmost, Cicero’s references to these characters without explicit mention of their names were not included in the final tally.

---

![alt text](https://raw.githubusercontent.com/wedebrockm/hacking-history-project/master/docs/imgs/included/Pictures%20for%20Project/Picture8.jpg)

---

While the above note is an enormous caveat, that would be the work of a much larger project, perhaps one that also included a more detailed analysis of the context in which these dynamics ensued.  Still, there are some cases from this sample that are worth mentioning.  Explicit mentions of Clodia and Atratinius are only mentioned as objects. The only exception to this rule is when Clodia’s name appears with Caelius.  This placement as an object might have enhanced Cicero’s invective.  While this is a curious phenomenon, without a deeper look at when Clodia is referenced as a pronoun rather than by name, this trend remains inconclusive due to sample size.  This assumption also seems more doubtful when one notes that Caelius’ name often appears as an object.  Instead, it seems more likely that he wanted those particular names to linger in the mind of his listeners.

Overall, rather than revealing as much about Cicero’s use of the active and passive voice in his invective, these numbers more depict Cicero's style. He seems to favor using names after the verb, and slightly favors using the passive voice over the active. This may reflect his affinity for participles during this period (Dyck 2013, 18-19). That he tends to place names at the end of his sentences may be a point of emphasis, or it may vary based on the exact context of each use.  Ultimately, this dataset provides more correlation than any direct causation due to the relatively small set of results and lack of absolute trends.  In some ways this is to be expected, however, for if Cicero's language is as complex and nuanced as we might think, it seems natural for it to be difficult to define his style on this single data set.

# Conclusion

The findings of this study demonstrate a few noteworthy concepts when it comes to applying digital methodologies to textual analyses. First, it seems clear that applied technologies, even though they are still even today in their infancy, have remarkable potential in allowing for a faster reading and analysis of texts. Once I learned how to utilize the web scraping tool, *Arakhne* to clean the text, and some advanced functions of the *Word* find tool, it was a straightforward process to scrape, scrub, and analyze the text itself. Admittedly, the simplicity of my approach handicapped my efforts in some regards, and as a result that I had to supplement these technologies with different strategies in order to realize the final project goals. A prime example of this would be searching for part of certain names that weren't in the existing work catalogue, or having to manually read portions of the text because there was no easy way to categorize participles using the find feature.  In retrospect, this project would have been aided by finding or creating tools for parsing the text itself for verb voice. This perhaps reveals some current holes in the field, as to my knowledge no such automated programs are available. Instead, digital methods must necessarily remain supplementary at the moment to traditional methods for parsing texts.

Still, the value of using digital tools in text analysis seems vindicated through how much time it saved.  Sifting through the entire *Pro Caelio* by hand would have required a substantially greater time investment when compared to compartmentalizing the text via *Arakhne* and *Web Scraper*.  Further, the *Pro Caelio* is a relatively short text, so the time saved would be multiplied on a massive scale if one attempted to translate a much larger work or corpuses of writings.  In sum, the digital field is a growing one, and as new technologies emerge the methodological field will continue to expand and become increasingly important for scholars to utilize, even for scholars focused on the more traditional historical topics.

---

# Bibliography

von Albrecht, Michael. 2003. *Cicero’s Style: A Synopsis.* Boston: Brill.

Argamon, Shlomo, Charles Cooney, Russell Horton, Mark Olsen, Sterling Stein, and Robert Voyer. 2009. "Gender, Race, and Nationality in Black Drama, 1950-2006: Mining Differences in Language Use in Authors and their Characters." *Digital Humanities Quarterly* 3(2). http://www.digitalhumanities.org/dhq/vol/3/2/000043/000043.html

Dyck, Andrew R. 2013. *Cicero: Pro Marco Caelio.* Cambridge: Cambridge University Press.

Cerutti, Steven M. 1999. *Cicero: Pro Archia Poeta Oratio: A Structural Analysis of the Speech and Companion to the Commentary.* Wauconda: Bolchazy-Carducci Publishers.

Leen, Anne. “Clodia Oppugnatrix: The Domus Motif in Cicero’s ‘Pro Caelio.’” *The Classical Journal* 96, no. 2 (2000): 141–162.

Manuwald, Gesine. 2014. *Cicero.* London: I.B.Tauris.

Patrik, Linda E. 2007. "Encoding for Endangered Tibetan Texts." *Digital Humanities Quarterly* 1(1). http://www.digitalhumanities.org/dhq/vol/1/1/000004/000004.html

Townsend, Robert B. 2013. "Openings and New PhDs on the Rise: The 2012 Jobs Report." *AHA: Perspectives on History*, January. https://www.historians.org/publications-and-directories/perspectives-on-history/january-2013/the-2012-jobs-report
