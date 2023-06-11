
<p align="center"><img src="https://github.com/lokesh-go/inferless/assets/31778886/0a30e5fd-cd57-48ab-bb1d-b72543d6d6e8" alt="Inferless" width="150px"/></p>

# Inferless

Serverless GPU offering to help with scaling machine learning inference without any hassle of managing servers.

## Sharing a very high level thoughts and understanding about the Inferless Product.

#### Steps to deploy Models:
- **Add Models** - _Choose this option to add a new model_
- **Select the Frameworks** - _Choose framework according to the model_
- **Import the Models** - _Import the models from remote or local file server_
- **Sync the Accounts** - _Listing remote repositories with OAuth login_
- **Create Model** - _Import custom model here with remote model link_
- **Runtime Configuration** - _Configure the runtime here like: sets MIN & MAX scalings_
- **Review & Deploy** - _Review & deploy the Models on the server_


#### Approach breakdown 
- ##### Add Models
  - ###### User View
    - Add Models (+) option will be available at FE, So user easily add their ML models with this option.
  - ###### Approach
    - ###### Basic
      - Simply Add Models option can be add with HTML, CSS or some other UI Framework at the Client side itself.
    - ###### Scalable
      - Whatever options we have to show on Front end, It can be handle at **Server side configurable**.
      - **All Metadata** which will show on Front end, It can be **powered by Backend APIs**.
      - Obviously, It is a heavy read opeartion then we can consider Caching here to handle **Millions of Request Per Minute**.

- ##### Select the Frameworks
  - ###### User View
    - Listing frameworks will be available at FE, So user can easily select the required Model's Framework.
  - ###### Approach
    - ###### Basic
      - All frameworks (_ONNX, TensorFlow, PyTorch etc ..._) listed on the Client side itself.
    - ###### Scalable
      - Same as above, It can be **powered by Backend APIs**.

##### Imports the Models
  - ###### User View
    - Repo importing feature are available on the FE, So user can import their Models from local or remote repo.
  - ###### Approach
      - All repo importing functionalities (_Local file, Github, Hugging Face Repo_):
        - ###### Local File
          - Simply we can attach any file browers which are already availables on the Client Side itself. (_HTML, CSS, Some other web frameworks_) 
        - ###### Github
          - Can avail this option with Github plugins on the Client Side.
        - ###### Hugging Face Repo
          - Can avail this option with Hugging Face plugins on the Client Side.

##### Sync the Accounts
  - ###### User View
    - User can sync & list their remote repositories on the Inferless to importing the Models from remote server.
  - ###### Approach
    - Can integrate the remote repo with OAuth login. User can esily gets their remote repositories lists on the Interless side with OAuth login.

##### Create Model
  - ###### User View
    - User can create a Model which he/she wants to execute on the serverless GPU. Take the required inputes from user like ( _model-name, model-type, task-type, model-url, sample-input, sample-output_ ).
  - ###### Approach
    - These options are available at the FE Client side or we can get these options values and metadata from server side.

##### Runtime Configuration
  - ###### User View
    - User can choose runtime like ( _PyTorch, ONNX etc ..._ ) and also set their Min & Max pod scaling value.
  - ###### Approach
    - Same these options can be handle at the FE or BE.


##### Review & Deploy
  - ###### User View
    - Final step where all selected options are available here to review. After review just click on Run or Deploy to start ML Models computing at the Server side.
  - ###### Approach
    - Here Can have final Deploy API to execute inputed ML Modules on the serverless GPU.

