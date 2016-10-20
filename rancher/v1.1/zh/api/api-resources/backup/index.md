---
title: API
layout: rancher-api-default-v1.1
version: v1.1
lang: zh
---

## backup



### Resource Fields

#### Writeable Fields

Field | Type | Create | Update | Default | Notes
---|---|---|---|---|---
description | string | Optional | Yes | - | 
name | string | Optional | Yes | - | 


#### Read Only Fields

Field | Type   | Notes
---|---|---
accountId | [account]({{site.baseurl}}/rancher/{{page.version}}/{{page.lang}}/api/api-resources/account/)  | The unique identifier for the associated account
backupTargetId | [backupTarget]({{site.baseurl}}/rancher/{{page.version}}/{{page.lang}}/api/api-resources/backupTarget/)  | 
created | date  | The date of when the backup was created.
id | int  | The unique identifier for the backup
kind | string  | 
removed | date  | The date of when the backup was removed
snapshotId | [snapshot]({{site.baseurl}}/rancher/{{page.version}}/{{page.lang}}/api/api-resources/snapshot/)  | 
state | enum  | The current state of the backup. The options are [created, creating, removed, removing, requested].
transitioning | enum  | Whether or not the backup is in a transitioning state
transitioningMessage | string  | The message to show while in a transitioning state
transitioningProgress | int  | The percentage remaining in the transitioning process of the backup
uri | string  | 
uuid | string  | The universally unique identifier for the backup. This will always be unique across Rancher installations.
volumeId | [volume]({{site.baseurl}}/rancher/{{page.version}}/{{page.lang}}/api/api-resources/volume/)  | 


<br>