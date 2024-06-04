# insights-ib-satellite-sync

This repo contains a job template that allows synchornisation of certain type of images from Red Hat Insights image builder to Red Hat Satellite. The purpuse is to have images created by Insights Image Builder available for longer time, as today they are available for 6 hours only. 

Please note: 

- it will sync only Guest images (QCOW2)
- It will take 2 parameters - client_id and client_secret (check service account creation for Red Hat Insights and provide the neccessary permissions to that account)
- You need to edit the job template to modify some of the variables


TO DO: 
- parametrize some of the other variables so that the job template can be used out of the box
- optimize the queries, as they are suboptimal right now
