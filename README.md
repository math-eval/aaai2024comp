# AAAI2024 Global Competition on Math Problem Solving and Reasoning


Both the TAL-SAQ7K-CN and TAL-SAQ6K-EN datasets for [AAAI2024 Global Competition on Math Problem Solving and Reasoning](https://ai4ed.cc/competitions/aaai2024competition) can be download here. The TAL-SAQ7K-CN and TAL-SAQ6K-EN datasets are used as the test sets for this competition. They consist of 7,436 and 5,927 questions respectively. Answers to the questions will not be disclosed.

Each question and its auxiliary information is stored in the JSON format with the following fields:

* “dataset_version”: The identifier of the source dataset version.
* “queId”: The identifier of the global ID for the question.
* “difficulty”: The difficulty level of the question, ranging from 0 to 4.
* “qtype”: The type of the question, with the value “short_answer” indicating that the question is a short answer question.
* “problem”: The question content of a math competition question.
* “knowledge_point_routes”: The knowledge point route from coarse-grained to fine-grained.

Here, we provide a real sample from TAL-SAQ6K-EN and TAL-SAQ7K-CN respectively.

**A math problem sample from TAL-SAQ6K-EN**
```
{
    "dataset_version": "2023-07-07",
    "queId": "17a4a261e09e46b188ed0705441570df",
    "difficulty": "3",
    "qtype": "short_answer",
    "problem": "In a number sequence, the first integer is $$3$$, the second is $$10$$, and starting from the third integer, each integer is the sum of the two integers directly in front of it. What is the remainder when the $$1997^{\\text{th}}$$ integer is divided by $$3$$? ",
    "knowledge_point_routes": ["Overseas Competition-&gt;Knowledge Point-&gt;Number Theory Modules-&gt;Remainder Problems-&gt;Questions involving Divisions with Remainders"]
}

```

**A math problem sample from TAL-SAQ7K-CN**
```
{
    "dataset_version": "2023-07-07",
    "queId": "05de5fa272834c0d91b4a9e60d3b9068",
    "difficulty": "4",
    "qtype": "short_answer",
    "problem": "一枚均匀的硬币掷$$10$$次，从不接连出现正面的概率为$$\\frac{i}{j}$$（即约分数），求$$i+j$$．",
    "knowledge_point_routes": ["竞赛-&gt;知识点-&gt;排列组合与概率-&gt;概率初步"]
}
```
In addition, the file **submission_example.json** is an example prediction result JSON file for submission, when submitting, **rename it as TAL_SAQ7K_CN_prediction.json**, and put it into a directory, then go inside the directory to do zip, and finally upload the zip file for submission.

### Licensing Information

The TAL-SAQ7K-CN and TAL-SAQ6K-EN datasets are licensed under the [MIT License](https://opensource.org/license/mit/)
