# Hate Detection (v 1.0.0)
![social](https://img.shields.io/github/followers/kshitijahande?style=social) ![language](https://img.shields.io/badge/python-v%203.8-neonorange) ![language](https://img.shields.io/badge/scikit__learn-v%200.24.2-9cf)


This is a repository for Hate Detection project under Research Methodology course Spring '21 at Lakehead University, Canada.


## Table of Contents

1. [Our Philosophy](#our-philosophy)
2. [About this project](#about-this-project)
3. [Road-map](#road-map)
4. [Project Status](#project-status)
5. [Manifest](#manifest)
6. [Dataset](#dataset)
7. [Results](#results)
8. [Support](#support)



## Our Philosophy 
Rising cases of online bullying via offensive and hateful comments or tweets online makes hate detection of upmost need in this era. Multiple millenials including celebs, have fallen prey to online bashing afftecting their mental health, increasing anxiety and depression. Our philosophy is to share LOVE not hate 💜

## About this project

- This project will help identify potential hate texts from non-hateful ones. 
- You can type a message or comment in the input box in UI and hit submit. It will then display either 'This comment is hurtful' or 'GOOD JOB! Please continue spreading love 💌 !' based on harshness of the language used.
- This feature can be  further enhanced to prevent the user from posting such comments and completely avoid the hastle of blocking a user and establish respectful boundaries.
- Its a plug and play feature, it can be integrated with your website user suggesion or comment box in a jiffy 🏃

## Road-map 
<!-- - Collect data from HateSpeech.org
- Clean data, remove punctuations, emojis, special characters and store this clean data aside
- Perform data analysis
- Tokenize with bert or n-gram
- Task 1 : Multiclass classification between hateful, offensive language and neither -->
- Task 2 : Include Sentiment classification task to improve classification accuracy
- Task 3 : Auto convert hateful words into endearing or encouraging antonyms and generate meaningful sentenses

## Project Status 

☑️ Collected data from HuggingFace library <br>
☑️ Cleaned data, removed punctuations, emojis, special characters like hash tags and Twitter user mentions <br>
☑️ Perform data analysis <br>
☑️ Tokenized with TF-IDF and n-gram <br>
☑️ Task 1 : Multiclass classification between hateful, offensive language and neither <br>


## Manifest

- A list of the top-level files in this project with a description of what each file is.

```
- README.md                                          ----> This markdown file you are reading.
- 1_classifier_tfidf_svc.ipynb                       ----> This is experiment #1 to achieve Task 1. It uses only TF-IDF with Logistic regression and Linear SVM 
- 2_classifier_tfidf_pos_logistic_regression.ipynb   ----> This is experiment #2 to achieve Task 1. It uses TF-IDF and POS tagging with Logistic regression and Linear SVM 
- 3_classifier_bert.ipynb                            ----> This is a in-progress experiment #3 to extract features using BERT tokenizer
```

## Dataset 

- This dataset is pulled from HuggingFace library, made available by [T. Davidson](https://huggingface.co/datasets/hate_speech_offensive)
- Total rows: 24,783
- Following columns are accessible:
```
'count',             --------> the number of CrowdFollower workers voted for class labelling
 'hate_speech_count',            --------> the number of CrowdFollower workers classified tweet as hate speech
 'offensive_language_count',     --------> the number of CrowdFollower workers classified tweet as offensive language
 'neither_count',             --------> the number of CrowdFollower workers classified tweet as neither hate speech nor offensive language
 'class',             --------> Final class label assigned to the tweet      
 'tweet'            --------> Tweet 

```
- Class column can contain values 0, 1 or 2
```
"class":[
            0:"hate speech"
            1:"offensive language"
            2:"neither"
]
```

## Results



## Support
 ![social](https://img.shields.io/badge/email%20me-job.kshitijahande%40gmail.com-blueviolet)

- I would highly appreciate and welcome all your contributions and suggestions to improve this work!
<!-- [email me](job.kshitijahande@gmail.com) -->


<!-- ## Necessary Things for a README

Depending on exactly what sort of project you are doing, there are a number of things that you may or may not want to include in a readme. There is really no **one true way** to do it. Readme's are a kind of _artform_.

*__However__* there are a few things that you should consider including:

1. Name of your project.
2. Description of your project.
3. Badges.
4. Graphics / Visuals
5. Install Instructions
6. Usage (how does one use the program once it is installed.)
7. Support / Contact Details.
8. Road-map (future ideas)
9. How to contribute
10. Authors / Acknowledgements (give credit where credit is due!)
11. License
12. Project Status


## Visuals

- Visuals are very important! You might want to include screenshots of your code in operation. GIFS are also great!
- Just use the "![ ]()" to input images.

## Installation 

- Describe how your software / development is installed. Sometimes it's easy as something like:

```bash
sudo apt-get install my-cool-thing
```

- often it involves a bit of  downloading sources and building:

```bash
git clone my-cool-repo.git
cd /my-cool-repo
cd /build
make
```

- You should list out steps as unambiguously as humanly possible!!
- Often people don't read the actual install instructions, but they just copy and paste what is in the black boxes. __Keep this in mind!__

## Usage

- Describe how the program / project is going to be used once it is installed.  If it is a command line app, you'll want to give CLI examples:

```bash
cool-project -arg1 -arg2
```

- then maybe show a screenshot of  the results :smile:

## License

- Depending on what kind of project you are doing, you might have a specific copyright. 
- Usually on github, everything is open source!
- You can find license info here: [license](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github/licensing-a-repository)

 -->





