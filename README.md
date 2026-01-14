## Telegram Social Network Dataset

This dataset represents a Telegram social network modeled as a graph, where users, bots, groups, and channels are connected through their interactions.
It is designed for Social Network Analysis (SNA), graph mining, and machine learning tasks such as influence detection, community discovery, and anomaly detection.

The dataset is stored in two files:

nodes.csv – describes the entities in the network

edges.csv – describes how those entities interact

📁 File Structure
dataset/
│
├── nodes.csv
└── edges.csv

📄 nodes.csv — Node Information

Each row in nodes.csv represents a Telegram entity such as a user, bot, group, or channel.

Columns
Column	Description
id-Unique identifier of the node
label	Name or label of the entity
type	Type of node (user, bot, group, channel)
members	Number of members (for groups or channels)
role	Role of the user (e.g., admin, moderator, member)
created_at	Creation date of the account or group
active_status	Whether the entity is active or inactive
age	Age of the user (if available)
gender	Gender of the user
location	Geographic location
language	Primary language used
topic	Main discussion topic or interest
category	Category of the group or channel
visibility	Whether the group/channel is public or private

This file provides node attributes that can be used for demographic analysis, behavior modeling, and filtering.

📄 edges.csv — Interaction Data

Each row in edges.csv represents an interaction between two Telegram entities.

Columns
Column	Description
source	ID of the sender or initiating node
target	ID of the receiving node
relation	Type of interaction (e.g., message, reply, forward)
weight	Strength or frequency of interaction
timestamp	Time when the interaction occurred
message_length	Length of the message
sentiment_score	Sentiment score of the message (negative to positive)
forwarded	Whether the message was forwarded (True / False)
group_channel_id	Group or channel where the interaction occurred

This file defines the edges of the graph and captures how information flows across the Telegram network.

Training graph-based machine learning models
