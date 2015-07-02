# twain-speak
Trains a character-based language model on novels using recurrent neural networks, to generate text in the style of Mark Twain.

# Setup
Pull the docker repo
```
docker pull mbartoli/char-rnn
```
and then open a shell within the container 
```
docker run -i -t CONTAINER_ID /bin/bash
```
Run
```
luarocks install nngraph
luarocks install optim
```
Next, clone this repo, and run setup.sh.  

# Training
To train, run  
```
sh train.sh 
```

# Sampling 
To generate text, edit ```sampling.sh``` and replace ```ENTER_CHECKPOINT_HERE``` with your model checkpoint found in ```/home/char-rnn/cv```.  Then run  
```
sh sampling.sh
```


# Additional Info
See  
https://github.com/karpathy/char-rnn  
http://karpathy.github.io/2015/05/21/rnn-effectiveness/

Docker  
https://github.com/mbartoli/docker-char-rnn  
https://registry.hub.docker.com/u/mbartoli/char-rnn/ 
