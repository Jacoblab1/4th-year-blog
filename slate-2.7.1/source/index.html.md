---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - java
  - xml

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/slatedocs/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true

code_clipboard: true
---

# Introduction

Welcome to SYSC 4907 Back-end Web Development. You can use this as a documentation to setup environment used in project.

# Setup
* To set up project using Eclipse first you need to go to the marketplace and download the EGit packages.

* Then install the proper JRE (JRE 8 in this case). 

Go to Eclipse -> preference -> Java -> Installed JRE -> selected JRE on PC. 

* Then go to Apache Tomcat https://tomcat.apache.org/ to download corresponding releases. 
Go to the download folder for Tomcat and navigate to the bin folder, grant access for all the .bat files. 
Catalina.bat, cipher.bat, configtest.bat, digest.bat, setclasspath.bat, shutdown.bat, startup.bat, tool-wrapper.bat and version.bat

* Execute the Tomcat start script

* Then import the project from github.
Go to File -> import -> Git -> Projects from Git -> clone URL or existing local repository if already cloned to local. -> your_destination_folder -> select project -> import. 

* Enable Maven depandencies
Go to Preference -> Maven -> enable Download repository index updates on startup option. 

* Restart eclipse. 

# Overall
The project contain three seperate projects - sim.parsing, sim.reise, sim.service. 

The file correspond to the code of one PUT method

```java 
@PutMapping(path="/Accounts/{username}")  
	public String createAccount(@PathVariable String username,@RequestBody String accountProperties) throws IOException  
	{
		int x =	service.createAccount(username,accountProperties);
		
		if (x==201) return "Status = 201 : Account Created";  
		
		else return "Status : " + Integer.toString(x) + "\n Problem occured while creating account";
	}

```

```xml
			<Files>	
			<File name="sower_manager.ma" type="MA" location="/"/>
			<File name="sower_manager.ev" type="EV" location="/"/>
			<File name="sower_manager.log" type="LOG" location="/"/>
			<File name="sower_manager.bat" type="BAT" location="/"/>
		</Files>
```




<!-- Kittn uses API keys to allow access to the API. You can register a new Kittn API key at our [developer portal](http://example.com/developers).


# Kittens

## Get All Kittens



<!-- ```shell
curl "http://example.com/api/kittens"
  -H "Authorization: meowmeowmeow"
``` -->
<!-- 
```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let kittens = api.kittens.get();
``` -->

> The above command returns XML structured like this:


This file illustrates a portion of xml file.

<!-- ### HTTP Request

`GET http://example.com/api/kittens`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Get a Specific Kitten

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get(2)
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get(2)
```

```shell
curl "http://example.com/api/kittens/2"
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let max = api.kittens.get(2);
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to retrieve

## Delete a Specific Kitten

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.delete(2)
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.delete(2)
```

```shell
curl "http://example.com/api/kittens/2"
  -X DELETE
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let max = api.kittens.delete(2);
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "deleted" : ":("
}
```

This endpoint deletes a specific kitten.

### HTTP Request

`DELETE http://example.com/kittens/<ID>`

### URL Parameters -->

