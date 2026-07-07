# gamedev_engines_sentiment_data
Repo for data of reddit sentiment around game engines

3 files are present:
extracted_data.jsonl: this is the raw data that the LLM outputted, I choose to not force strict schema here to let the results be more natural
extracted_data_normalized.jsonl: this is the normalized data, raw data modeled into topics and sub-topics (using an LLM based script and some manual tunning), here some categories aren't normalized or are normalized very poorly because there weren't enough data for them in the first place (I found it not useful to focus on them too much), these fields are project_type and developer_persona, the rest I spent a lot of time on.
normalization_config.json: this is the config that maps raw user text to the topics and sub-topics.
