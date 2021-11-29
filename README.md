# Animal Classification solution using AML(azure machine learning)&ADF(azure data factory)&iot edge 

## prerequisite 

1. azure machine learning desginer 
2. azure data factory
3. iot edge

## Azure machine learning 

In this part, Using azure machine learning designer to train the Animal classification task with Resnet, the whole experiment is:

![image](https://user-images.githubusercontent.com/36184365/143800557-25944bb8-e519-420c-bdc5-11e4b8a4e75c.png)

Dataset: Animal images dataset

NN:Resnet

ML infra: Pytorch

In the designer, we create a pipeline as shown in picture above, Once it could be ran successfully and we could publish it and a pipeline endpoint as:

![image](https://user-images.githubusercontent.com/36184365/143800984-a5b6d7ce-3887-4c8d-b86b-3a2521b4f78c.png)

The result is:
![image](https://user-images.githubusercontent.com/36184365/143801130-6b3bb828-e2fc-4122-9efb-7601cac94ee5.png)

This is what we could use on ADF part to triggr the pipeline running automatically using the exposed REST endpoint for example:
https://eastus.api.azureml.ms/pipelines/v1.0/subscriptions/XXXXX/resourceGroups/github/providers/Microsoft.MachineLearningServices/workspaces/github/PipelineRuns/PipelineEndpointSubmit/Id/XXXXX

## Azure data factory

## Iot edge


For more information about sparse checkout please visit [this](https://stackoverflow.com/questions/23289006/on-windows-git-error-sparse-checkout-leaves-no-entry-on-the-working-directory) stackoverflow thread.

## Code of Conduct
This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## License
These samples and templates are all licensed under the MIT license. See the license.txt file in the root.

## Questions
Email questions to: zezhan@microsoft.com.
