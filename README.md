<h1>Quora-question-pair-similarity</h1>
<h2> Business Problem</h2>
<p>
Quora is a place to gain and share knowledge—about anything. It’s a platform to ask questions and connect with people who contribute unique insights and quality answers. This empowers people to learn from each other and to better understand the world.</p>
<p>Over 100 million people visit Quora every month, so it's no surprise that many people ask similarly worded questions. Multiple questions with the same intent can cause seekers to spend more time finding the best answer to their question, and make writers feel they need to answer multiple versions of the same question. Quora values canonical questions because they provide a better experience to active seekers and writers, and offer more value to both of these groups in the long term.</p>
<P>Credits: Kaggle</p>
<h2>Problem Statement</h2>
Identify which questions asked on Quora are duplicates of questions that have already been asked.
<h2>Real world/Business Objectives and Constraints</h2>
<ol>
<li>The cost of a mis-classification can be very high.</li>
<li>You would want a probability of a pair of questions to be duplicates so that you can choose any threshold of choice.</li>
<li>No strict latency concerns.</li>
<li>Interpretability is partially important.</li>
  </ol>
<h2>Data Overview</h2>
Data will be in a file Train.csv
<ul>
<li>Train.csv contains 5 columns : qid1, qid2, question1, question2, is_duplicate. </li>
<li>Size of Train.csv - 60MB</li>
<li>Number of rows in Train.csv = 404,290. </li>
  </ul>
<h2>Mapping the real world problem to an ML problem</h2>
It is a binary classification problem, for a given pair of questions we need to predict if they are duplicate or not.
<h2> Performance Metric</h2>
<ol>
  <li>Log-loss </li>
  <li>Binary Confusion Matrix</li>
  </ol>
