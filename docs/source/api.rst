APIs
--------------------------


.. py:class:: CS2D(penalty='l2', backdoor_penalty = 0.1, sele_penalty = 0.1, class_weight = None, random_state=None, solver='Adam', max_iter=100, pre_trained = None)

   :param float backdoor_penalty: The mangnitude of the penalty on the backdoor loss
   :param float sele_penalty: The mangnitude of the penalty on the selection mechanism
   :param int random_state: RandomState instance; Used when solver == ‘sag’, ‘saga’ or ‘liblinear’ to shuffle the data
   :param str solver: The person sending the message
   :param int max_iter: Maximum number of iterations taken for the solvers to converge
   :param str pre_trained: Specify the path of a pre-trained model
   
   
   
   .. py:method:: fit(X, y, backdoor_target, sample_weight = None)
        
        Fit the model according to the given training data.
        
        :param arr X: The person sending the message
        :param arr y: The recipient of the message
        :param str backdoor_target: The target class
        
   
   .. py:method:: selection(X, y, backdoor_target, sample_weight = None)
        
        Fit the model according to the given training data.
        
        :param arr X: The person sending the message
        :param arr y: The recipient of the message
        :param str backdoor_target: The target class
        
        
   .. py:method:: predict(X, y, backdoor_target, sample_weight = None)
        
        Fit the model according to the given training data.
        
        :param arr X: The person sending the message
        :param arr y: The recipient of the message
        :param str backdoor_target: The target class



.. py:function:: send_message(sender, recipient, message_body, [priority=1])

   Send a message to a recipient

   :param str sender: The person sending the message
   :param str recipient: The recipient of the message
   :param str message_body: The body of the message
   :param priority: The priority of the message, can be a number 1-5
   :type priority: integer or None
   :return: the message id
   :rtype: int
   :raises ValueError: if the message_body exceeds 160 characters
   :raises TypeError: if the message_body is not a basestring


.. py:class:: example_numpy.py

