
## 4.3 Confusion table

<a href="https://www.youtube.com/watch?v=Jt2dDLSlBng&list=PL3MmuxUbc_hIhxl5Ji8t4O6lPAOpHaCLR"><img src="images/thumbnail-4-03.jpg"></a>
 

[Slides](https://www.slideshare.net/AlexeyGrigorev/ml-zoomcamp-4-evaluation-metrics-for-classification)


## Notes

Confusion table is a way of measuring different types of errors and correct decisions that binary classifiers can make. Considering this information, it is possible to evaluate the quality of the model by different strategies.

When comes to a prediction of an LR model, each falls into one of four different categories:

* Prediction is that the customer WILL churn. This is known as the **Positive class**
    * And Customer actually churned - Known as a **True Positive (TP)**
    * But Customer actually did not churn - Known as a **False Positive (FP)**
* Prediction is that the customer WILL NOT churn' - This is known as the **Negative class**
    * Customer did not churn - **True Negative (TN)**
    * Customer churned - **False Negative (FN)**

'Confusion Table' is a way to summarize the above results in a tabular format, as shown below: 

<table>
  <thead>
    <tr>
      <th></th>
      <th colspan="2"><b>Predictions</b></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b>Actual</b></td>
      <td><b>Negative</b></td>
      <td><b>Positive</b></td>
    </tr>
   <tr>
      <td><b>Negative</b></td>
      <td>TN</td>
      <td>FP</td>
    </tr>
    <tr>
      <td><b>Positive</b></td>
      <td>FN</td>
      <td>TP</td>
    </tr>
  </tbody>
</table>

![confusion_matrix.png](images%2Fconfusion_matrix.png)

The **accuracy** corresponds to the sum of TN and TP divided by the total of observations. 

The code of this project is available in [this jupyter notebook](notebook.ipynb).  

Add notes from the video (PRs are welcome)

<table>
   <tr>
      <td>⚠️</td>
      <td>
         The notes are written by the community. <br>
         If you see an error here, please create a PR with a fix.
      </td>
   </tr>
</table>

* [Notes from Peter Ernicke](https://knowmledge.com/2023/10/04/ml-zoomcamp-2023-evaluation-metrics-for-classification-part-3/)

## Navigation

* [Machine Learning Zoomcamp course](../)
* [Session 4: Evaluation Metrics for Classification](./)
* Previous: [Accuracy and dummy model](02-accuracy.md)
* Next: [Precision and Recall](04-precision-recall.md)
