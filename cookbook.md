---
title: "Codebook for Getting and Cleaning Data Assignment"
output: html_document
---
        
This codebook.md contains three sections including 
        1.) Data
        2.) Variable
        3.) Transformation
See *Readme.md* for data information and background.

## Data  
the tidy dataset is located in this repository, *Tidy_data.txt*.
The first row contains names of variable, descripting in variable section, and the following rows contains the values of each variables.

## Variable
subject : range from 1 to 30

activity : there are 6 activities including  
        1. WALKING  
        2. WALKING_UPSTAIRS  
        3. WALKING_DOWNSTAIRS  
        4. SITTING  
        5. STANDING  
        6. LAYING  
  
Measurements : the measurements are collected from either accelerometer and gyrometer. Also, the magnitude of these three-dimensional signals were calculated using the Euclidean norm.

The measurements are divided into two domain
        1. time-domain signals is resulted from accelerometer and gyrometer.
        2. frequency-domain signals is resulted from the application of a Fast         Fourier Transform (FFT) to some of the time-domain signals.
        
### Time-domain signals  
* Average time-domain body acceleration in the X, Y and Z directions:  
    + timeDomainBodyAccelerometerMeanX  
    + timeDomainBodyAccelerometerMeanY  
    + timeDomainBodyAccelerometerMeanZ  
* Standard deviation of the time-domain body acceleration in the X, Y and Z directions:
    + timeDomainBodyAccelerometerStandardDeviationX
    + timeDomainBodyAccelerometerStandardDeviationY
    + timeDomainBodyAccelerometerStandardDeviationZ
* Average time-domain gravity acceleration in the X, Y and Z directions:
    + timeDomainGravityAccelerometerMeanX
    + timeDomainGravityAccelerometerMeanY
    + timeDomainGravityAccelerometerMeanZ
* Standard deviation of the time-domain gravity acceleration in the X, Y and Z directions:
    + timeDomainGravityAccelerometerStandardDeviationX
    + timeDomainGravityAccelerometerStandardDeviationY
    + timeDomainGravityAccelerometerStandardDeviationZ
* Average time-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
    + timeDomainBodyAccelerometerJerkMeanX
    + timeDomainBodyAccelerometerJerkMeanY
    + timeDomainBodyAccelerometerJerkMeanZ
* Standard deviation of the time-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
    + timeDomainBodyAccelerometerJerkStandardDeviationX
    + timeDomainBodyAccelerometerJerkStandardDeviationY
    + timeDomainBodyAccelerometerJerkStandardDeviationZ
* Average time-domain body angular velocity in the X, Y and Z directions:
    + timeDomainBodyGyroscopeMeanX
    + timeDomainBodyGyroscopeMeanY
    + timeDomainBodyGyroscopeMeanZ
* Standard deviation of the time-domain body angular velocity in the X, Y and Z directions:
    + timeDomainBodyGyroscopeStandardDeviationX
    + timeDomainBodyGyroscopeStandardDeviationY
    + timeDomainBodyGyroscopeStandardDeviationZ
* Average time-domain body angular velocity jerk (derivation of the angular velocity in time) in the X, Y and Z directions:
    + timeDomainBodyGyroscopeJerkMeanX
    + timeDomainBodyGyroscopeJerkMeanY
    + timeDomainBodyGyroscopeJerkMeanZ
* Standard deviation of the time-domain body angular velocity jerk (derivation of the angular velocity in time) in the X, Y and Z directions:
    + timeDomainBodyGyroscopeJerkStandardDeviationX
    + timeDomainBodyGyroscopeJerkStandardDeviationY
    + timeDomainBodyGyroscopeJerkStandardDeviationZ
* Average and standard deviation of the time-domain magnitude of body acceleration:
    + timeDomainBodyAccelerometerMagnitudeMean
    + timeDomainBodyAccelerometerMagnitudeStandardDeviation
* Average and standard deviation of the time-domain magnitude of gravity acceleration:
    + timeDomainGravityAccelerometerMagnitudeMean
    + timeDomainGravityAccelerometerMagnitudeStandardDeviation
* Average and standard deviation of the time-domain magnitude of body acceleration jerk (derivation of the acceleration in time):
    + timeDomainBodyAccelerometerJerkMagnitudeMean
    + timeDomainBodyAccelerometerJerkMagnitudeStandardDeviation
* Average and standard deviation of the time-domain magnitude of body angular velocity:
    + timeDomainBodyGyroscopeMagnitudeMean
    + timeDomainBodyGyroscopeMagnitudeStandardDeviation
* Average and standard deviation of the time-domain magnitude of body angular velocity jerk (derivation of the angular velocity in time):
    + timeDomainBodyGyroscopeJerkMagnitudeMean
    + timeDomainBodyGyroscopeJerkMagnitudeStandardDeviation

### Frequency-domain signals
* Average frequency-domain body acceleration in the X, Y and Z directions:
    + frequencyDomainBodyAccelerometerMeanX
    + frequencyDomainBodyAccelerometerMeanY
    + frequencyDomainBodyAccelerometerMeanZ
* Standard deviation of the frequency-domain body acceleration in the X, Y and Z directions:
    + frequencyDomainBodyAccelerometerStandardDeviationX
    + frequencyDomainBodyAccelerometerStandardDeviationY
    + frequencyDomainBodyAccelerometerStandardDeviationZ
* Weighted average of the frequency components of the frequency-domain body acceleration in the X, Y and Z directions:
    + frequencyDomainBodyAccelerometerMeanFrequencyX
    + frequencyDomainBodyAccelerometerMeanFrequencyY
    + frequencyDomainBodyAccelerometerMeanFrequencyZ
* Average frequency-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
    + frequencyDomainBodyAccelerometerJerkMeanX
    + frequencyDomainBodyAccelerometerJerkMeanY
    + frequencyDomainBodyAccelerometerJerkMeanZ
* Standard deviation of the frequency-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
    + frequencyDomainBodyAccelerometerJerkStandardDeviationX
    + frequencyDomainBodyAccelerometerJerkStandardDeviationY
    + frequencyDomainBodyAccelerometerJerkStandardDeviationZ
* Weighted average of the frequency components of the frequency-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
    + frequencyDomainBodyAccelerometerJerkMeanFrequencyX
    + frequencyDomainBodyAccelerometerJerkMeanFrequencyY
    + frequencyDomainBodyAccelerometerJerkMeanFrequencyZ
* Average frequency-domain body angular velocity in the X, Y and Z directions:
    + frequencyDomainBodyGyroscopeMean
    + frequencyDomainBodyGyroscopeMeanY
    + frequencyDomainBodyGyroscopeMeanZ
* Standard deviation of the frequency-domain body angular velocity in the X, Y and Z directions:
    + frequencyDomainBodyGyroscopeStandardDeviationX
    + frequencyDomainBodyGyroscopeStandardDeviationY
    + frequencyDomainBodyGyroscopeStandardDeviationZ
* Weighted average of the frequency components of the frequency-domain body angular velocity in the X, Y and Z directions:
    + frequencyDomainBodyGyroscopeMeanFrequencyX
    + frequencyDomainBodyGyroscopeMeanFrequencyY
    + frequencyDomainBodyGyroscopeMeanFrequencyZ
* Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body acceleration:
    + frequencyDomainBodyAccelerometerMagnitudeMean
    + frequencyDomainBodyAccelerometerMagnitudeStandardDeviation
    + frequencyDomainBodyAccelerometerMagnitudeMeanFrequency
* Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body acceleration jerk (derivation of the acceleration in time):
    + frequencyDomainBodyAccelerometerJerkMagnitudeMean
    + frequencyDomainBodyAccelerometerJerkMagnitudeStandardDeviation
    + frequencyDomainBodyAccelerometerJerkMagnitudeMeanFrequency
* Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body angular velocity:
    + frequencyDomainBodyGyroscopeMagnitudeMean
    + frequencyDomainBodyGyroscopeMagnitudeStandardDeviation
    + frequencyDomainBodyGyroscopeMagnitudeMeanFrequency
* Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body angular velocity jerk (derivation of the angular velocity in time):
    + frequencyDomainBodyGyroscopeJerkMagnitudeMean
    + frequencyDomainBodyGyroscopeJerkMagnitudeStandardDeviation
    + frequencyDomainBodyGyroscopeJerkMagnitudeMeanFrequency

## Transformation
The run_analysis.R is the script performing 5 steps including  
1. File downloading and preparation: this step is about download the UCI HAR Database (as .zip) and unzip it into specific path.  
2. Applying variable.  
3. Merging dataset including train set, test set, and subject.  
4. Labeling with appropiated names.  
5. Making the tidy data set.  

