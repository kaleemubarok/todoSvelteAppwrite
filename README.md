# 🔖 Todo With Svelte

A simple todo app built with Appwrite and Svelte modified from: [Appwrite Repository](https://github.com/appwrite/demo-todo-with-svelte)

If you simply want to try out the App, go ahead and check out the demo at https://todo.oil.my.id/

## 🎬 Getting Started

### 🤘 Install Appwrite 
Follow our simple [Installation Guide](https://appwrite.io/docs/installation) to get Appwrite up and running in no time. You can either deploy Appwrite on your local machine or, on any cloud provider of your choice. 

> Note: If you setup Appwrite on your local machine, you will need to create a public IP so that your hosted frontend can access it.
  
We need to make a few configuration changes to your Appwrite server. 

1. Add a new Web App in Appwrite and enter the endpoint of your website (`localhost, <project-name>.vercel.app etc`)
![Appwrite Console](https://user-images.githubusercontent.com/31401437/155891052-09bb17e4-a30c-4c73-8c9f-b1cc0b44c596.png)

2. Create a new collection with the following properties
* **Attributes**
Add the following attributes to the collection. 
> Make sure that your Attribute ID exactly matches the key in the images

<p align="center">
<img src="https://user-images.githubusercontent.com/42211/155337647-41ca47a3-9b5b-4853-bca0-f22815e60228.png" alt="Content Attribute" width="400"/>
</p>

<p align="center">
<img src="https://user-images.githubusercontent.com/42211/155338065-5b8349e9-e4c9-4be5-a407-04ce7c5b3c4f.png" alt="IsComplete Attribute" width="400"/>
</p>

* **Permissions**
Add the following permissions to your collections. These permissions ensure that only registered users can access the collection.

<p align="center">
<img src="https://user-images.githubusercontent.com/20852629/113019801-99bc1580-919f-11eb-9a94-13b1529cb925.png" alt="Collection Permissions" width="400"/>
</p>

### 🚀 Deploy the Front End
You have two options to deploy the front-end and we will cover both of them here. In either case, you will need to fill in these environment variables that help your frontend connect to Appwrite.

* VITE_APP_ENDPOINT - Your Appwrite endpoint
* VITE_APP_PROJECT - Your Appwrite project ID
* VITE_APP_COLLECTION_ID - Your Appwrite collection ID 

### **Run locally**

Follow these instructions to run the demo app locally

```sh
$ git clone https://github.com/appwrite/todo-with-svelte
$ cd todo-with-svelte
```

Run the following command to generate your `.env` vars  

```sh
$ cp .env.example .env
```

Now fill in the envrionment variables we discussed above in your `.env`

Now run the following commands and you should be good to go 💪🏼 
```
$ npm install
$ npm run dev
```
