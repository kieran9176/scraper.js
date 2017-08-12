# scraper.js

Scraper.js traverses a user-given Wikipedia article, finds all of the hyperlinks in that article, and returns an array of objects containing:
  1. the keyword from each hyperlink
  2. the number of occurences of that keyword in the article
  3. the hyperlink itself

The results begin with the links from the first paragraph, followed by the links that are most common throughout the rest of the article (sorted in descending order).

Example: 'neural network' returns

[ { name: 'Connectionism',
    numOccur: 4,
    link: '/wiki/Connectionism' },
    
  { name: 'Biological neural network',
    numOccur: 4,
    link: '/wiki/Biological_neural_network' },
    
  { name: 'Labeled data', numOccur: 1, link: '/wiki/Labeled_data' },
  
  { name: 'Rule-based programming',
    numOccur: 1,
    link: '/wiki/Rule-based_programming' },
    
  { name: 'Convolution', numOccur: 51, link: '/wiki/Convolution' },
  
  { name: 'Boltzmann machine',
    numOccur: 26,
    link: '/wiki/Boltzmann_machine' },
    
  { name: 'Backpropagation',
    numOccur: 25,
    link: '/wiki/Backpropagation' },
    
  { name: 'Statistic', numOccur: 24, link: '/wiki/Statistic' },
  
  { name: 'Gradient', numOccur: 22, link: '/wiki/Gradient' },
  
  { name: 'Neural network',
    numOccur: 20,
    link: '/wiki/Neural_network' },
    
  { name: 'Machine learning',
    numOccur: 16,
    link: '/wiki/Machine_learning' },
    
  { name: 'Tensor', numOccur: 16, link: '/wiki/Tensor' },
  
  { name: 'Brain', numOccur: 14, link: '/wiki/Brain' },
  
  { name: 'Hebbian', numOccur: 13, link: '/wiki/Hebbian' },
  
  { name: 'Restricted Boltzmann machine',
    numOccur: 13,
    link: '/wiki/Restricted_Boltzmann_machine' },
    
  { name: 'Supervised learning',
    numOccur: 12,
    link: '/wiki/Supervised_learning' },
    
  { name: 'Convolutional neural network',
    numOccur: 12,
    link: '/wiki/Convolutional_neural_network' },
    
  { name: 'Encoder', numOccur: 11, link: '/wiki/Encoder' },
  
  { name: 'Deep belief network',
    numOccur: 11,
    link: '/wiki/Deep_belief_network' },
    
  { name: 'Synapse', numOccur: 10, link: '/wiki/Synapse' },
  
  { name: 'Unsupervised learning',
    numOccur: 10,
    link: '/wiki/Unsupervised_learning' },
    
  { name: 'Turing machine',
    numOccur: 10,
    link: '/wiki/Turing_machine' },
  
  etc ... ]
