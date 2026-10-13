# AI Healthcare: Symptom Information Checker

## Project Overview

For this project, I created a simple healthcare application using Python and Natural Language Processing (NLP). The goal of this project was to learn how NLP can be used in healthcare to recognize symptoms from text entered by users.

The application allows users to describe their symptoms in their own words. It then processes the text, identifies common symptoms, and displays general information about them.

I also added a separate triage demonstration that uses fictional patient examples to show how a rule-based system can classify different situations.

## Tools and Technologies

- **Python:** Used to write the application.
- **NLP:** Used to process text and recognize symptoms.
- **Regular Expressions (Regex):** Used to search for symptoms and identify simple negative statements.
- **Gradio:** Used to create the application interface.
- **Google Colab:** Used to write and test the code.

## How the Application Works

The application follows a few basic steps:

1. The user enters a sentence describing their symptoms.
2. The application converts the text to lowercase.
3. It searches for symptoms using a small symptom database.
4. It recognizes different forms of words, such as "headache" and "headaches."
5. It tries to separate symptoms the user reports having from symptoms they say they do not have.
6. It displays the recognized symptoms and general health information.

For example, if the user enters:

"I have coughing and nausea, but no headache."

The application should recognize:

- **Reported symptoms:** Cough and nausea
- **Denied symptom:** Headache

The application also includes a separate section with fictional examples that demonstrate preliminary assessments and triage levels using Python rules.

## What I Learned

Through this project, I learned how NLP can be used to process information related to healthcare. I practiced working with Python dictionaries, loops, functions, and regular expressions.

I also learned how to create a simple web interface using Gradio and connect it to my Python code.

One of the interesting parts was learning how important negative words are. For example, "I have a fever" and "I do not have a fever" have different meanings. This showed me why processing medical text correctly is important.

## Testing

I tested the application using different example sentences to see if it could identify symptoms correctly.

I also included automated tests to check common symptom matches, negative expressions, and the fictional triage examples.

These tests help check whether the code works as expected, but they do not prove that the application is medically accurate.

## Limitations

This application is a simple educational project, so it has some limitations.

It only recognizes symptoms included in its database and may not understand complicated sentences. It uses basic NLP rules rather than a trained machine learning model.

The application cannot provide an accurate medical diagnosis or determine whether a real patient needs emergency care.

## Privacy and Ethical Considerations

Privacy and accuracy are important when using AI in healthcare. For this project, I used fictional examples instead of real patient information.

The application is not designed to collect or store medical records. However, information entered into a hosted application may still be processed by the hosting service.

The application also includes a disclaimer explaining that it is for educational purposes only and should not replace professional medical advice.

## How to Run the Project

1. Open Google Colab.
2. Upload the `AI_Healthcare_Colab.ipynb` notebook.
3. Run the cells from top to bottom.
4. Wait for the Gradio interface to appear.
5. Enter an example symptom description and click the button to analyze it.
6. Explore the fictional triage examples in the separate section.

## References

1. *Natural language processing of symptoms documented in free-text narratives of electronic health records: A systematic review.* (2019).  
https://pmc.ncbi.nlm.nih.gov/articles/PMC6657282/

2. World Health Organization. (2021). *Ethics and governance of artificial intelligence for health.*  
https://www.who.int/publications/i/item/9789240029200

3. NLTK Documentation.  
https://www.nltk.org/

4. Gradio Documentation.  
https://www.gradio.app/docs

## Disclaimer

This application was created for educational purposes only. It is not intended to provide medical diagnoses, treatment recommendations, or real medical triage decisions. Anyone with medical concerns should consult a qualified healthcare professional.
