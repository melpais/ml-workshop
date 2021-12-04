# ML Workshop - December 9th 2021
![Agenda](./images/agenda.png)


## Ingest, Prepare and Feature Store

Use the following command to clone the [workshop](https://github.com/data-science-on-aws/oreilly_book)
```
git clone https://github.com/data-science-on-aws/oreilly_book.git
```

*Introduction*
* <span style="color:purple">01_introduction/01_Setup_Dependencies.ipynb</span>.
* <span style="color:purple">01_introduction/02_Check_Environment.ipynb</span>.
* <span style="color:purple">01_introduction/03_Create_S3_Bucket.ipynb</span>.
* <span style="color:purple">01_introduction/04_Update_IAM_Roles_And_Policies.ipynb</span>.

*Ingest*
* 04_ingest/00_Overview.ipynb
* 04_ingest/01_Copy_TSV_To_S3.ipynb
* 04_ingest/02_Create_Athena_Database.ipynb
* 04_ingest/03_Register_S3_TSV_With_Athena.ipynb
* 04_ingest/04_Convert_S3_TSV_To_Parquet_With_Athena.ipynb

*Explore*
* 05_explore/00_Overview.ipynb
* <span style="color:purple">05_explore/01_Visualize_Reviews_Dataset.ipynb</span>.

*Prepare*
* 06_prepare/00_Overview.ipynb
* <span style="color:purple">06_prepare/01_Prepare_Dataset_BERT_Scikit_AdHoc_FeatureStore.ipynb</span>. (10m)
  - It takes about 6 minutes for *data to be availabe in offline feature store* 
  - If you get any errors due to Athena limits, simply rerun the step.
* <span style="color:purple">06_prepare/02_Prepare_Dataset_BERT_Scikit_ScriptMode_FeatureStore.ipynb</span>. (20m)
  - The processing job takes 15 minutes to run
  - If you get any errors due to Athena limits, simply rerun the step and it should work fine.

## Train, Model Registry, and Deployment and AutoScaling
*Train*
- 07_train/00_Overview.ipynb
- 07_train/01_Train_Reviews_BERT_Transformers_TensorFlow_AdHoc.ipynb
- 07_train/02_Train_Reviews_BERT_Transformers_TensorFlow_ScriptMode.ipynb

*Deploy*
- 09_deploy/00_Overview.ipynb
- 09_deploy/03_Deploy_Reviews_BERT_TensorFlow_REST_Endpoint.ipynb
- 09_deploy/04_Autoscale_Reviews_BERT_TensorFlow_REST_Endpoint.ipynb

## SageMaker Pipelines, EKS/Kubeflow ML Pipeline
- 10_pipeline/00_Overview.ipynb
- 10_pipeline/01_Create_SageMaker_Pipeline_BERT_Reviews.ipynb
- 10_pipeline/05_Register_Deploy_Model.ipynb
- 10_pipeline/kubeflow



Resources:
- [Dive deep into Amazon SageMaker Studio Notebooks architecture](https://aws.amazon.com/blogs/machine-learning/dive-deep-into-amazon-sagemaker-studio-notebook-architecture/)