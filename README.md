In this project I use HMMs to decode American Sign Language from short videos and I go over three different methods (CV, BIC and DIC) to select the optimal number of states for each model. An accuracy of 55% is achieved (vocabulary size = 112 words) using the Bayesian Information Criterion.

The data in the `asl_recognizer/data/` directory is derived from 
the [RWTH-BOSTON-104 Database](http://www-i6.informatik.rwth-aachen.de/~dreuw/database-rwth-boston-104.php). 
The right/left hand and nose positions (`hand_condensed.csv`) are pulled directly from 
the database [boston104.handpositions.rybach-forster-dreuw-2009-09-25.full.xml](boston104.handpositions.rybach-forster-dreuw-2009-09-25.full.xml).

The videos are sentences with translations provided in the database. The sentences have been pre-segmented into words 
based on slow motion examination of the files. These segments are contained in the `train_words.csv` and `test_words.csv` files
in the form of start and end frames (inclusive). Training and testing word files have been divided as they are in the database.

The videos in the corpus include recordings from three different ASL speakers.
The mappings for the three speakers to video are included in the `speaker.csv` 
file.

This is an adaptation of a project carried out in the context of the Artificial Intelligence Nanodegree by Udacity.
