# AI-900 Study Notes - Day 2

## Machine Learning

**Deep Learning**: an advanced subset of ML that uses **neural networks with many layers** (deep neural networks) to learn complex patterns and excels at tasks like **image recognition** and natural language understanding. It often requires **large amounts of data and computational power**.

**Neural Networks**: loosely **simulate interconnected “neurons” in the human brain**, adjusting weights through training to recognize patterns.

**Automated Machines Learning** is a feature in Azure Machine Learning that **automatically tries different algorithms** and hyperparameters to train models on your data, aiming to **find the best model without extensive manual tuning**. This saves time by automating model selection and optimization (works with **Supervised Machine Learning only**). You can also choose to use either the **Python SDK or a no-code user interface** to build an AutoML experiment.

**Real time Deployment**: Designed for **low-latency responses**, ideal for scenarios requiring **immediate predictions**.

**Batch Processing Deployment**: Best for large-scale inference at **lower operational costs**, suitable for **non-time-sensitive workloads**.

**Compute Scheduling** helps **optimize** resource usage by automatically **shutting down compute instances when idle**, reducing unnecessary costs.

**Workspaces** are the **starting point** for Azure Machine Learning, serving as the **central hub** for all your ML activities.

**Data Transformation**: include **Cleaning the missing data**, **Normalizing the data**, **select the columns of interest** in the data set.

**Azure ML Experiment** is a logical container for one or more runs (executions of your code) within an Azure ML workspace, you can choose a **primary metric used to compare the results of individual experimental runs**, and **a list of blocked algorithms that should be excluded from the training runs**.

**Job** is the **actual execution** of some ML work: training, evaluation, pipeline step, or script run.

**Azure Machine Learning Designer** is a **draganddrop, nocode/lowcode interface** inside Azure Machine Learning Studio that lets you visually build **machine learning pipelines** without writing code.

**Inferencing pipeline** is a workflow that **uses a trained model to generate predictions** on new, unseen data.

**Endpoint** in Azure Machine Learning is a **stable, durable HTTPS URL** that applications can call to send input data to a **deployed ML model or pipeline**, and receive prediction outputs, it's how your trained model becomes usable in the real-world using **REST API** and **Authentication Key**.

### � Azure ML Workflow Steps

**Step 0**: **Create a workspace** to be able to use any Azure ML Service (AutoML, Designer,...)

**Step 1**: **Create a new ML Job** and select the appropriate task type, such as regression or classification.

**Step 2**: **Choose which columns** from your dataset to include or exclude for analysis.

**Step 3**: **Select the primary metrics** you want to use for evaluating model performance, and exclude any algorithms you do not wish to use.

**Step 4**: **Identify and select the target column** (label) that you want to predict.

**Step 5**: **(Featurization)** by cleaning up missing information and normalizing values as needed.

**Step 6**: **Choose the compute resources** for your job, such as serverless, CPU, or GPU options.

**Step 7**: **Review the output results** and deploy your model to an endpoint.

### �📝 ML Quick Reference

| Component            | Key Points                                                                                                 |
| -------------------- | ---------------------------------------------------------------------------------------------------------- |
| **Azure AutoML**     | • Python SDK or no-code user interface<br>• Supervised ML only<br>• Automatically select best ML algorithm |
| **Batch Processing** | • Lower operational costs in Azure ML                                                                      |
| **Compute Clusters** | • Dedicated: guaranteed nodes<br>• Low-priority: not guaranteed nodes                                      |
| **Model Usage**      | • REST endpoint + authentication key                                                                       |
| **Scheduling**       | • Shut down when idling (cost optimization)                                                                |

## Computer Vision

### 🔍 Core Vision Tasks

#### Image Classification

**Categorizes** an image into **one of several classes** by analyzing an image and outputs a label (or labels) **describing the main content**.

#### Object Detection

Identifies and **locates multiple objects within an image** and classifies these objects and **draws bounding boxes** around each detected object **with a confidence score**.

#### Optical Character Recognition (OCR)

**Extracts text from images** and converts it into machine-readable text.

#### Custom Vision

Allows **training custom image classification or object detection** models using your own data.

#### Semantic Segmentation

A computer vision technique that **classifies every individual pixel in an image** according to the object or region it belongs to.

### 👥 Face & Video Analytics

#### Face API

**Detects faces**, compares for similarity, and **identifies people from a labeled database**. It returns **face landmarks** and **accessories worn by the subject (attributes)**.

#### Video Analysis Service

Supports **Spatial Analysis**, which lets you **analyze video streams from camera devices in real time**. For each camera device you configure, the Spatial Analysis operations will generate an output stream of **JSON messages**.

#### Azure AI Video Indexer

A cloud application, part of Azure AI services, built on Azure AI services (such as the Face, Translator, Azure AI Vision, and Speech). It enables you to **extract the insights from your videos** using Azure AI Video Indexer video and audio models. It's perfect for making the videos **searchable** and **identify key historical events of general interests**.

### 📝 Computer Vision Quick Reference

| Component            | Key Details                                                                                                                                                         |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Custom Image**     | • Max file size = 6 MB                                                                                                                                              |
| **Object Detection** | • Bounding box with confidence score                                                                                                                                |
| **Face API**         | • Outputs JSON file<br>• Face landmarks and accessories/attributes<br>• No eye/skin color data<br>• one-to-many: Face Identification; one-to-one: Face verification |
| **Video Analysis**   | • Spatial analysis capabilities                                                                                                                                     |
| **Image Analysis**   | • Celebrities, landmarks, brands (prebuilt/predefined)                                                                                                              |
| **AI Video Indexer** | • Searchable and identify key historical events                                                                                                                     |
| **Detection Tasks**  | • Face/Object "Detection" → bounding box                                                                                                                            |
