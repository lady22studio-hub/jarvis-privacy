---
layout: default
title: My home Jarvis Privacy Policy
---

# Privacy Policy for My home Jarvis Alexa Skill

Last updated: October 21, 2026

## Scope and operator

My home Jarvis is a personal Alexa skill operated by the owner of the lady22studio-hub GitHub account. It is intended solely for the operator's own use and is not currently offered for use by other people. This policy describes how information is handled when that personal skill is used. Publishing this policy does not make the skill available to the public.

Privacy contact: [lady22studio@gmail.com](mailto:lady22studio@gmail.com).

## Information processed and stored

The skill processes task text supplied through Alexa and the results generated when those tasks are processed. Its backend stores a hashed Alexa user identifier, task text, and task results. A hashed identifier is a pseudonymous identifier; hashing does not make the associated task text or results anonymous. Task text and results may contain personal information included in the request or generated in response.

Alexa supplies request information to the skill backend, including a user identifier that is used to derive the stored hash. The storage of a hashed identifier does not mean the original identifier is never processed while handling a request.

## How the system uses information

Information is used to receive and identify requests, queue tasks, execute tasks, associate results with the requesting user, and provide responses.

The system uses AWS Lambda for backend request processing, Amazon SQS for task queuing, Amazon DynamoDB for stored records, and a Windows Worker for task execution. Task data therefore passes through AWS services and the computer running the Windows Worker.

Task text is also sent to OpenAI to process requests and generate results. This includes personal information contained in that text. OpenAI is an external service provider, so information sent to it is processed outside the operator's local Windows environment.

## External services

Amazon processes Alexa interactions under its own terms and privacy notices. AWS provides the cloud services used by this skill, and OpenAI processes task text submitted to its service. Their processing, storage locations, and retention practices depend on the services used, applicable terms, and account configuration. This policy does not promise a particular retention period, deletion outcome, or model-training setting for those providers.

For information about these providers, see [Amazon's Privacy Notice](https://www.amazon.com/privacy), [AWS Data Privacy](https://aws.amazon.com/compliance/data-privacy/), and [OpenAI's Privacy Policy](https://openai.com/policies/privacy-policy/).

## Retention

No fixed retention period or automatic deletion schedule is specified in this policy for the skill's stored records. Do not assume that completing a task, receiving a response, or disabling the skill deletes previously stored information. Queued messages, database records, local Worker data, and any logs or backups may have different lifecycles depending on the actual system configuration.

## Data deletion requests

Deletion requests can be sent to [lady22studio@gmail.com](mailto:lady22studio@gmail.com) and are handled manually by the operator. Include an approximate usage time and a non-sensitive task description to help locate the relevant records. Do not send passwords, AWS access keys, OpenAI API keys, or other credentials.

The operator will verify the request and identify the associated records before taking deletion action. The review covers relevant DynamoDB records, any local Windows Worker records, and whether related tasks remain queued in SQS. The operator will explain the records that can be deleted and any limitations that apply to logs, backups, or copies held by external providers. This policy does not guarantee immediate deletion, a fixed completion deadline, or deletion of every copy across all systems.

Disabling the skill stops further use through Alexa but is not itself a request to delete previously stored records. Managing Alexa history with Amazon does not by itself delete the skill's backend records; deleting backend records does not by itself delete Amazon's or OpenAI's records.

## Changes and contact

This policy will be updated to reflect changes to the skill's actual data handling. If the skill is made available to other people, its data practices and this policy must be reviewed before that change.

For privacy questions or deletion requests, contact [lady22studio@gmail.com](mailto:lady22studio@gmail.com).
