# Reinforcement Learning with Human Feedback (RLHF) for Text Summarization

This project explores the use of **Reinforcement Learning with Human Feedback (RLHF)** to enhance **text summarization tasks**, focusing on both advanced techniques and resource-efficient approaches. The project investigates how RLHF can be applied to abstractive summarization, leveraging human preferences to guide model behavior.

## Key Concepts
- **RLHF**: Reinforcement Learning with Human Feedback integrates human preferences to improve the model’s decision-making during training.
- **Abstractive Summarization**: A summarization approach where the model generates summaries using its own understanding, as opposed to extractive summarization that relies on copying parts of the source text.
- **PPO (Proximal Policy Optimization)**: A reinforcement learning algorithm used in this project for fine-tuning models to generate better summaries.
- **DPO (Direct Preference Optimization)**: Another method used to directly optimize model behavior based on human feedback.

## Dataset
- **OpenAI/SummarizeFromFeedback**: This dataset was used to fine-tune the models. It contains human feedback on generated summaries, which is crucial for RLHF-based training.

## Models Evaluated
- **Reward Models**: Models trained to assign a reward to generated summaries.
- **Supervised Fine-Tuned (SFT) Models**: Models fine-tuned with human feedback to generate summaries.
- **PPO Models**: Reinforcement learning-based models fine-tuned with PPO for better performance in abstractive summarization tasks.

## Challenges Addressed
- **Memory Limitations with Large Models**: Challenges with scaling large models (e.g., 7B parameters) were mitigated using techniques like gradient accumulation and quantization.
- **Model Scalability**: Comparisons were made with smaller models, such as Gemma-2B, to evaluate their effectiveness as reward classifiers, despite their limited generative capabilities.

## Algorithmic Exploration
- **Reinforcement Learning Algorithms**: The project evaluated the effectiveness and stability of various RL algorithms such as A2C, A3C, and TRPO. The limitations of these algorithms in terms of scalability and stability were discussed.
- **PPO Performance**: The trade-offs between resource usage and performance were explored, with PPO showing significant improvements in summarization quality.

## Results and Insights
- **Gemma-2B**: This smaller model performed exceptionally well in classification tasks and was effective as a reward classifier.
- **PPO for Summarization**: PPO was found to significantly improve the quality of generated summaries, offering a balance between performance and resource efficiency.
- **Resource-Model Alignment**: One key insight is that model selection should be aligned with available computational resources to maximize efficiency and output.

## Future Directions
- **Testing Alternative RL Algorithms**: Future work will explore other RL algorithms, such as **ILQL**, to improve model performance.
- **Scaling Models**: Further experimentation with scaling models to optimize performance while managing resource consumption.
- **Expanding RLHF Applications**: The application of RLHF to other fields, such as **robotics**, will also be explored to expand its versatility.

## Setup and Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/JaishreeramCoder/Masters-Thesis-Project1.git
   cd Masters-Thesis-Project1
