# Customer Complaints v0.1 (CuCom) Dataset

A multilingual dataset of ~10,000 customer service conversations between users and AI assistants in the banking and insurance domain.

## Description
This dataset contains **synthetic user-agent conversations** in JSON format, simulating customer complaint resolution scenarios. Each entry represents a dialogue between a frustrated customer (user) and a customer support agent (LLM-based assistant), covering issues like investment delays, extra charges, insurance claims, card blocking, and service failures.

### Format
```json
{
  "id": "conv_9855",
  "turns": [
    {"role": "user", "content": "..."},
    {"role": "assistant", "content": "..."}
  ]
}
```

## Objective
- Train/fine-tune LLMs for **multilingual customer support**
- Benchmark models on **code-mixed language understanding**
- Develop systems for **emotional tone handling** in customer service
- Study **cross-lingual intent recognition** in real-world scenarios

## Languages
1. **Hindi (Devanagari script)**
2. **Hinglish** (Hindi-English code-mixing)
3. **Transliterated Hindi** (Roman script)
4. **English**

## Dataset Details
| Parameter       | Value                     |
|-----------------|---------------------------|
| Conversations   | 9,858                    |
| Avg Turns/Dialogue | 8-16                      |
| Domains         | Banking, Insurance        |
| Total turns | 136642 |
| Text Characteristics | Emotional language, slang, code-switching |

## Key Use Cases
1. **Multilingual Chatbot Training**
   - Handle code-mixed customer queries
   - Manage frustrated/angry user tones

2. **Sentiment Analysis**
   - Detect urgency/frustration in complaints
   - Emotion-aware response generation

3. **Intent Recognition**
   - Classify complaint types (SIP delays, card blocking, etc)
   - Entity extraction (account numbers, claim IDs)

4. **Cultural NLP Research**
   - Study code-switching patterns
   - Analyze informal financial vocabulary

## Getting Started
1. **Download Dataset**
   ```bash
   wget https://github.com/vakyansh/cucom/raw/refs/heads/main/data/cucuom_v1.jsonl.zip
   ```


## License
[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)

## Contributing
We welcome contributions through:
- Additional annotations (emotion labels, intent tags)
- Improved translations
- More conversation samples
- More Domain

Please open an issue or PR if you want to request any additional domain.


**Note**: Sensitive information (account numbers, phone numbers) in samples is fictionalized. Real user identifiers have been anonymized.
