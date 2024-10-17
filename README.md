# Investigating Intra-Layer Neuronal Mechanisms

This project implements and investigates intra-layer neuronal mechanisms within spiking neural networks, such as **Lateral Inhibition**, **k-Winners-Take-All (KWTA)**, and **Homeostasis**, using the **CoNeX framework**. The goal is to explore their effects on learning processes and network behavior in spiking neural networks trained with the **Spike-Timing-Dependent Plasticity (STDP)** learning rule.

## Table of Contents
- [Project Overview](#project-overview)
- [Implemented Features](#implemented-features)
- [How to Run](#how-to-run)
- [Results](#results)
- [References](#references)

## Project Overview
This project focuses on understanding the role of intra-layer neuronal mechanisms, such as **Lateral Inhibition**, **KWTA**, and **Homeostasis**, in shaping the behavior of spiking neural networks. By implementing these mechanisms and evaluating their effects on learning, we aim to enhance the differentiation of patterns and improve the learning processes within the network. The network architecture involves input and output layers, with input patterns encoded using Poisson encoding.

## Implemented Features
1. **Lateral Inhibition**:
   - A mechanism that enhances pattern differentiation by inhibiting neighboring neurons in the output layer, making neurons more sensitive to spatially varying stimuli.
   
2. **k-Winners-Take-All (KWTA)**:
   - A competitive mechanism that selects the top K neurons with the highest activity, enhancing the learning of distinct patterns in classification tasks.

3. **Homeostasis**:
   - A regulatory process that maintains equilibrium in neuronal activity by adjusting weights and neuron responses, ensuring stable learning and preventing network over-excitation.

4. **STDP Learning Rule**:
   - Spike-Timing-Dependent Plasticity is used to adjust synaptic weights based on the timing of spikes, reinforcing connections that contribute to a neuron’s firing while weakening less useful connections.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/MohaZamani/Intra-Layer-Neuronal-Mechanisms.git
2. Install the necessary dependencies:
   ```bash
   pip install -r requirements.txt
3. Run the simulation notebooks:
   - **For Lateral Inhibition**: Open and run `lateral_inhibition.ipynb`
   - **For KWTA Mechanism**: Open and run `kwta.ipynb`
   - **For Homeostasis**: Open and run `homeostasis.ipynb`

   You can launch the notebooks by executing:
   ```bash
   jupyter notebook
## Results
Results from the simulations include:
- **Weight Evolution**: Plots showing how synaptic weights change in response to different input patterns and learning mechanisms.
- **Cosine Similarity**: A measure of similarity between weight vectors during learning, providing insight into the differentiation of patterns.
- **Neuron Activity**: Spike raster plots that visualize the activity of neurons across different experiments and mechanisms.

All simulation results  and detailed analysis is available in the [report](./Report/Report-P04.pdf).


## References
- **CoNeX Framework**: [GitHub Repository for CoNeX Framework](https://github.com/cnrl/CoNeX)
- **STDP Learning**: [Spike-Timing-Dependent Plasticity on Wikipedia](https://en.wikipedia.org/wiki/Spike-timing-dependent_plasticity)
- **Homeostasis**: [Homeostasis in Neural Networks](https://bio.libretexts.org/Bookshelves/Introductory_and_General_Biology/Book:_General_Biology_(Boundless)/33:_The_Animal_Body-_Basic_Form_and_Function/33.11:_Homeostasis_-_Homeostatic_Process)
