1. **Overview** of the analysis: Explain the purpose of this analysis.

   The purpose of this analysis is to predict the success of an applicant for funding  using the features as provided in the data set.

2. **Results**: Using bulleted lists and images to support your answers, address the following questions.

  * Data Preprocessing

    * What variable(s) are considered the target(s) for your model?
      *  Column 'IS_SUCCESSFUL' in the dataframe 'df'
    * What variable(s) are considered to be the features for your model?
      * Columns ['APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', 'ASK_AMT']
    * What variable(s) are neither targets nor features, and should be removed from the input data?
      * Columns ['EIN', 'NAME']

  * Compiling, Training, and Evaluating the Model

    * How many neurons, layers, and activation functions did you select for your neural network model, and why?

      * First hidden layer with 100 neurons with relu activation.

      * Second hidden layer with 30 neurons with sigmoid activation.

      * Third hidden layer with 10 neurons with sigmoid activation.

      * Output layer with 1 neurons with sigmoid activation.

        I tried using16 neurons in 2 hidden layers and tried again with 3 hidden layers with more neurons to check if the accuracy changes, but it did not change.

    * Were you able to achieve the target model performance?

      * No, the target performance (72%) remained less than 75% accuracy

    * What steps did you take to try and increase model performance?

      * designed a kerastuner model with different parameters to loop through for the activation, layers and neurons to check if the accuracy changes.

3. **Summary**: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.