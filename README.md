# "Share Love not Hate" - Assessing Hate Speech Detection methods using TF-IDF and POS tagging approach on Twitter (v 1.0.0)
![social](https://img.shields.io/github/followers/kshitijahande?style=social) ![language](https://img.shields.io/badge/python-v%203.8-neonorange) ![language](https://img.shields.io/badge/scikit__learn-v%200.24.2-9cf)

![gif](https://media.giphy.com/media/QNlKSoNIyfY3MT3fzI/giphy.gif)

This is a repository for Hate Detection project under Research Methodology course Spring '21 at Lakehead University, Canada.


## Table of Contents

1. [Our Philosophy](#our-philosophy)
2. [About this project](#about-this-project)
3. [Road-map](#road-map)
4. [Project Status](#project-status)
5. [Usage](#usage)
6. [Manifest](#manifest)
7. [Dataset](#dataset)
8. [Results](#results)
9. [Support](#support)



## Our Philosophy 
Rising cases of online bullying via offensive and hateful comments or tweets online makes hate detection of upmost need in this era. Multiple millenials including celebs, have fallen prey to online bashing afftecting their mental health, increasing anxiety and depression. Our philosophy is to share LOVE not hate 💜

![sloth](https://media.giphy.com/media/OocLVILtd7ybm/giphy.gif)

<!-- ![phone](https://media.giphy.com/media/l4pT49ce47qFBdVT2/giphy.gif) -->

<!-- ![miranda](https://media.giphy.com/media/5oH9MgEQSW2AM/giphy.gif) -->

## About this project

- This project will help identify potential hate texts from non-hateful ones. 
- You can type a message or comment in the input box in UI and hit submit. It will then display either 'This comment is hurtful' or 'GOOD JOB! Please continue spreading love 💌 !' based on harshness of the language used.
- This feature can be  further enhanced to prevent the user from posting such comments and completely avoid the hastle of blocking a user and establish respectful boundaries.
- Its a plug and play feature, it can be integrated with your website user suggesion or comment box in a jiffy 🏃

![sticker](https://media.giphy.com/media/bkocUWOVuyDkMVRvxM/giphy.gif) 

## Project Status 

☑️ Collected data from HuggingFace library <br>
☑️ Cleaned data, removed punctuations, emojis, special characters like hash tags and Twitter user mentions <br>
☑️ Perform data analysis <br>
☑️ Tokenized with TF-IDF with n-gram <br>
☑️ Tokenized with POS tagging with n-gram <br>
☑️ Task 1 : Multiclass classification between hateful, offensive language and neither <br>

## Road-map 
<!-- - Collect data from HateSpeech.org
- Clean data, remove punctuations, emojis, special characters and store this clean data aside
- Perform data analysis
- Tokenize with bert or n-gram
- Task 1 : Multiclass classification between hateful, offensive language and neither -->
- Task 2 : Include Sentiment classification task to improve classification accuracy
- Task 3 : Auto convert hateful words into endearing or encouraging antonyms and generate meaningful sentenses

## Usage
- No setup needed, just a google account 😺
- You can directly open each ipynb Notebook in this repository by copying the notebook to your personal drive to get started on Google Colab!
- "2_classifier_tfidf_pos_logistic_regression.ipynb" contains code for the best performing model
- The dataset is pulled in the .ipynb notebook itself so there is no need to explicitly copy data files
- If you wish to contribute, clone this repository
```
git clone 'https://github.com/kshitijahande/Hate-Detection.git'
```

## Manifest

- A list of the top-level files in this project with a description of what each file is.

```
- README.md                                          ----> This markdown file you are reading.
- 1_classifier_tfidf_svc.ipynb                       ----> This is experiment #1 to achieve Task 1. It uses only TF-IDF with Logistic regression and Linear SVM 
- 2_classifier_tfidf_pos_logistic_regression.ipynb   ----> This is experiment #2 to achieve Task 1. It uses TF-IDF and POS tagging with Logistic regression and Linear SVM 
- 3_classifier_bert.ipynb                            ----> This is a in-progress experiment #3 to extract features using BERT tokenizer
- documentation                                      ----> This folder contains all documentation work
- documentation/report.pdf
- documentation/slides.pdf
- results                                            ----> This folder contains detailed results for experiments #1 and # 2 table 
```

## Dataset 

- This dataset is pulled from HuggingFace library, made available by [T. Davidson](https://huggingface.co/datasets/hate_speech_offensive)
- Total rows: 24,783
- Following columns are accessible:
```
'count',             --------> the number of CrowdFlower workers voted for class labelling
 'hate_speech_count',            --------> the number of CrowdFlower workers classified tweet as hate speech
 'offensive_language_count',     --------> the number of CrowdFlower workers classified tweet as offensive language
 'neither_count',             --------> the number of CrowdFlower workers classified tweet as neither hate speech nor offensive language
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

- The experiment #2 using TF-IDF and POS tagging with Logistic regression for feature selection and Linear SVM for classification with L2 regularization performed the best, resulting in 0.91 F1-score.


![results](https://github.com/kshitijahande/Hate-Detection/blob/d46ad1ec5415a0b8d63b40cd3b01854bb9a5dadd/results/table_exp_1-2.png)


## Support
 ![social](https://img.shields.io/badge/email%20me-job.kshitijahande%40gmail.com-blueviolet)

- I would highly appreciate and welcome all your contributions and suggestions to improve this work!
<!-- [email me](job.kshitijahande@gmail.com) -->

![cat](https://media.giphy.com/media/2tSodgDfwCjIMCBY8h/giphy.gif)
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





