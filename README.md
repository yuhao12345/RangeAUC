# RangeAUC

The receiver operator characteristic (ROC) curve and the area
under the curve (AUC) are widely used to compare the performance
of different anomaly detectors. They mainly focus
on point-based detection. However, the detection of collective
anomalies concerns two factors: whether this outlier is
detected and what percentage of this outlier is detected. The
first factor is not reflected in the AUC. Another problem is the
possible shift between the anomaly score and the real outlier
due to the application of the sliding window. To tackle these
problems, we incorporate the idea of range-based precision
and recall, and suggest the range-based ROC and its counterpart
in the precision-recall space, which provides a new
evaluation for the collective anomalies.

RangeAUC is a generalized version of
AUC for the subsequence outlier with the following goals:
* Inertial to the boundary of subsequence outlier. a high
anomaly score near the border of outlier should be rewarded.
* Sensitive to the short subsequence outlier detection. failing to detect a short subsequence should be penalized.

## Example

Examples are available in example_RangeAUC.ipynb

## Comparison between AUC and rangeAUC 

* The mismatch between the anomaly score and subsequence anomaly.
<img width="500" src="./docs/img/tods_logo.png" alt="Logo" />
