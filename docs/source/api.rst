================
 APIs
================

.. py:class:: CS2D(backdoor_penalty = 0.1, selec_penalty = 0.1, class_weight = None, random_state=None, solver='Adam', max_iter=100, pre_trained = None)
 :param float backdoor_penalty: The mangnitude of the penalty on the backdoor loss
 :param float selec_penalty: The mangnitude of the penalty on the selection mechanism
 :param int random_state: RandomState instance; Used when solver == ‘sag’, ‘saga’ or ‘liblinear’ to shuffle the data
 :param str solver: The person sending the message
 :param int max_iter: Maximum number of iterations taken for the solvers to converge
 :param str pre_trained: Specify the path of a pre-trained model
   
       
.. py:method:: fit(X, y, backdoor_target)
        
        Fit the model according to the given training data.
        
        
        :param X: Training vector, where n_samples is the number of samples and n_features is the number of features
        :type X: array-like, sparse matrix of shape (n_samples, n_features)
        
        :param y: Target vector relative to X.
        :type y: array-like
        
        :param backdoor_target: Backdoor Target.
        :type backdoor_target: array-like
        
        :return: fitted estimator
        :rtype: self

        
        
.. py:method:: predict(X)
        
        Predict class labels for samples in X.
        
        :param arr X: Test samples.
        
        :return: Vector containing the class labels for each sample
        :rtype: array-like, sparse matrix
        
        :raises TypeError: if the X is not array/array-like
        

                                             
             
        
   .. py:method:: score(X, y)
       
        Return the mean accuracy on the given test data and labels.
        
        :param arr X: Test samples.
        :param arry y: True labels for X.
        
        :return: Mean accuracy of self.predict(X) wrt. y.
        :rtype: float
        
.. note::  The above predict and score methods serve for general prediction/inference purposes.


        
   .. py:method:: backdoor_selection(X, cutoff)
        
        Return the index of selected backdoor sample for given cutoff value.
        
        :param arr X: Test samples.
        :param float cutoff: The cutoff value for choosing backdoor samples.
        
        :return: Indices of selected data
        :rtype: array
        
.. note::
          The cutoff value should be in range :math:`(0,1)`.
        
   
   .. py:method:: backdoor_score(X, backdoor_target, cutoff)
        
        Return the mean accuracy on the given test data and labels.
        
        :param arr X: Test samples.
        :param str backdoor_target: Backdoor Target.
        :param float cutoff: The cutoff value for choosing backdoor samples.
        
        :return: Mean accuracy of self.predict(backdoor_selection(X, cutoff)) wrt. to backdoor_target
        :rtype: float
        
        
.. warning::
          This methods only concerns the accuracy on selected samples.




 










