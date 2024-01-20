<h2> Overview</h2>
<p>
This Python program implements a spam classifier using a Multilayer Perceptron (MLP) model. The classifier is trained to classify emails as either spam or ham (non-spam) using the <a href="https://spamassassin.apache.org/old/publiccorpus/">Apache SpamAssassin public data</a>. The MLP model is chosen for its high efficacy in terms of precision and recall. The program is designed to be easily executable without any additional files or dependencies, as the required files will be automatically downloaded by the included Jupyter notebook.
</p>

<h2>Project Files</h2>
<p>
The project includes the following files:
</p>
<h4>Executable File:</h4>
<ul>
  <li><b>spam-classifier-optimized.ipynb</b> - A Jupyter Notebook containing all the necessary functions for training, testing, and classifying emails. This file includes all the required functions for performing classification operations.
  </li>
</ul>
<h4>Result Files:</h4>
<ul>
  <li><b>evaluation.txt</b> - Contains the evaluation results table, including the Confusion Matrix of the spam and ham classes.</li>
  <li><b>spam_classifier_best.sav</b> - Contains the weights of the most optimized model.</li>
  <li><b>confusion_matrix.png</b> - Visual representation of the Confusion Matrix for the final results.</li>
</ul>

<h2>Pipeline</h2>
<p>
The development of the spam classifier program follows the following stages, as outlined in the attached Jupyter Notebook:
</p>
<ol>
  <li>Download the dataset.</li>
  <li>Data preparation:
    <ul>
      <li>Remove email headers, including sender details, receiver details, subject, and date.</li>
      <li>Convert the entire email to lowercase.</li>
      <li>Replace all URLs in the email with the word 'URL'.</li>
      <li>Replace all numbers in the email with the word 'NUM'.</li>
      <li>Remove all punctuation marks from the email.</li>
    </ul>
  </li>
  <li>Split the dataset into training and test sets.</li>
  <li>Convert the text data into a bag-of-words representation, which is a vector of word counts for each training instance.</li>
  <li>Train and evaluate the MLP model based on recall, precision, and the Receiver Operating Characteristic (ROC) curve.</li>
  <li>Fine-tune the MLP classifier.</li>
  <li>Evaluate the classifier on the test set.</li>
</ol>

<h2> Technologies Used </h2>
<p align="center"> 
  <img src="https://github.com/devicons/devicon/blob/master/icons/python/python-original.svg" alt="python" width="50" height="50"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/pandas/pandas-original-wordmark.svg" alt="pandas" width="50" height="50"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/numpy/numpy-original.svg" alt="numpy" width="50" height="50"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/jupyter/jupyter-original.svg" alt="jupyter" width="50" height="50"/>
  <img src="https://github.com/scikit-learn/scikit-learn/blob/main/doc/logos/scikit-learn-logo-notext.png" alt="scikit-learn" width="90" height="50"/>
  <img src="Images/matplotlib_logo.png" alt="matplotlib-logo" width="150" height="50"/>
</p>
