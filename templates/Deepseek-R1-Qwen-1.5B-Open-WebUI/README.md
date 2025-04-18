A high-throughput and memory-efficient inference engine for running DeepSeek's R1-Qwen-1.5B model using vLLM.
With a front end to communicate with the model via OpenAI-compatible API and a web UI for easy interaction.

## Description

This template provides an OpenAI-compatible API server for the R1-Qwen-1.5B model, optimized for performance using vLLM. This model is based on Qwen2.5-Math-1.5B and fine-tuned with DeepSeek-R1 samples, offering efficient performance for lightweight deployments.

It also provides a web UI for easy interaction with the model. The web UI is built using [Open-WebUI](https://github.com/open-webui/open-webui), allowing users to input prompts and receive responses from the model in a user-friendly interface.

## Usage Recommendations (from DeepSeek)

We recommend adhering to the following configurations when utilizing the DeepSeek-R1 series models, including benchmarking, to achieve the expected performance:

- Set the temperature within the range of 0.5-0.7 (0.6 is recommended) to prevent endless repetitions or incoherent outputs.
- Avoid adding a system prompt; all instructions should be contained within the user prompt.
- For mathematical problems, it is advisable to include a directive in your prompt such as: "Please reason step by step, and put your final answer within \boxed{}."
- When evaluating model performance, it is recommended to conduct multiple tests and average the results.

## Model Details

- **Name**: R1-Qwen-1.5B
- **Base Model**: Qwen2.5-Math-1.5B
- **Size**: 1.5 billion parameters

## Usage

The API follows the OpenAI API format and can be accessed via HTTP requests to port 9000. The model is served with the name "R1-Qwen-1.5B".

And the Open-WebUI is accessible on port 8000 after starting the server.

## License

This model is derived from Qwen-2.5 series and is licensed under Apache 2.0 License. The model has been fine-tuned with 800k samples curated with DeepSeek-R1. The model weights and code are available for commercial use.

## Links

- [DeepSeek R1 GitHub Repository](https://github.com/deepseek-ai/DeepSeek-R1)
-[Open-WebUI][https://github.com/open-webui/open-webui]
- [vLLM Documentation](https://github.com/vllm-project/vllm)

