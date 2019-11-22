# Continuous-Control
In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

Solution : The agent should get more than 30.0 for 100 consecutive episodes.

## Getting Started

### Download the Unity Environment

For this project, you will not need to install Unity - this is because we have already built the environment for you, and you can download it from one of the links below. You need only select the environment that matches your operating system:

Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)

Then, place the file in the folder in the Continuous-Control GitHub repository, and unzip (or decompress) the file.

### Output

<img src="/gif.gif" width= 500 px/>

### Instructions

 1. Download the project materials from my GitHub repository. You can download the repository with
  ```
  git clone https://github.com/vickipedia6/Continuous-Control.git
  ```
 2. Download anaconda or miniconda based on the instructions in the [Anaconda documentation](https://docs.anaconda.com).
 
 3. Create a new conda environment:
  ```
  conda create --name deep-learning python=3
  ```
 4. Enter your new environment:
  * Mac/Linux: >> ``` source activate deep-learning ```
  * Windows: >>  ```activate deep-learning ```
  
 5. Ensure you have numpy, matplotlib, pandas, and jupyter notebook installed by doing the following:
  ```
  conda install numpy matplotlib pandas jupyter notebook
  ```
 6. Run the following to open up the notebook server:
  ```
  jupyter notebook navigation.ipynb
  ```
 7. Execute all the cells in the code
 
### Project results

* The agent achieved the average score of 30.065 in less than 200 episodes.

<img src="/plot.png" width= 700 px/>

## Built With

* Python 3

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* The data comes from the Udacity.
