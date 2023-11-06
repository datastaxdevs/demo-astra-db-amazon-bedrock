# Getting Started with Amazon BedRock and AstraDB

[![License Apache2](https://img.shields.io/hexpm/l/plug.svg)](http://www.apache.org/licenses/LICENSE-2.0)
[![Discord](https://img.shields.io/discord/685554030159593522)](https://discord.com/widget?id=685554030159593522&theme=dark)

## 📋 Table of content

<img src="./img/banner.png" align="right" width="400px"/>

### Amazon BedRock

- [01. Chat Playground](#)
- [02. Prompt Engineering](#)
- [02. Prompt Templates](#)

### DataStax Astra DB

- [01. Create Astra Account](#-1---create-your-datastax-astra-account)
- [02. Create Astra Token](#-2---create-an-astra-token)
- [03. Copy the token](#-3---copy-the-token-value-in-your-clipboard)
- [04. Open Gitpod](#-4---open-gitpod)
- [05. Setup CLI](#-5---set-up-the-cli-with-your-token)
- [06. Create Database](#-6---create-destination-database-and-a-keyspace)
- [07. Setup env variables](#-7---setup-env-variables)

### Rag demo with


## Amazon Bedrock

In this tutorial we will work with Amazon Bedrock on within the Amazon Management Console 

![](./img/bedrock-00.png)

#### ✅ `1` - Chat Playground

- `1a` - Connect to your `AWS Management Consolee` and look for service `Amazon Bedrock`

![](./img/bedrock-01.png)

- On home page select getting started

![](./img/bedrock-02.png)

- In the left hand side menu pick `Chat`

- Select model Provider and model

| Attribute | Value |
|-----------|-------|
| Provider  | Anthropic |
| Model     | Claude V2 |

![](./img/bedrock-03-chat.png)

- In the prompt enter the question

```console
human: Explain me what Datastax Astra Vector is
```

![](./img/bedrock-04-chat.png)


#### ✅ `2` - Prompt Engineering




## AstraDB


#### ✅ `1` - Create your DataStax Astra account

> ℹ️ Account creation tutorial is available in [awesome astra](https://awesome-astra.github.io/docs/pages/astra/create-account/)


_click the image below or go to [https://astra.datastax./com](bit.ly/3QxhO6t)_

<a href="bit.ly/3QxhO6t">
<img src="https://awesome-astra.github.io/docs/img/astra/astra-signin-github-0.png" />
</a>
<br/>



#### ✅ `2` - Create an Astra Token

> ℹ️ Token creation tutorial is available in [awesome astra](https://awesome-astra.github.io/docs/pages/astra/create-token/#c-procedure)

- `Locate `Settings` (#1) in the menu on the left, then `Token Management` (#2)

- Select the role `Organization Administrator` before clicking `[Generate Token]`

![](https://github.com/DataStax-Academy/cassandra-for-data-engineers/blob/main/images/setup-astra-2.png?raw=true)

The Token is in fact three separate strings: a `Client ID`, a `Client Secret` and the `token` proper. You will need some of these strings to access the database, depending on the type of access you plan. Although the Client ID, strictly speaking, is not a secret, you should regard this whole object as a secret and make sure not to share it inadvertently (e.g. committing it to a Git repository) as it grants access to your databases.

```json
{
  "ClientId": "ROkiiDZdvPOvHRSgoZtyAapp",
  "ClientSecret": "fakedfaked",
  "Token":"AstraCS:fake"
}
```

#### ✅ `3` - Copy the token value in your clipboard

You can also leave the windo open to copy the value in a second.