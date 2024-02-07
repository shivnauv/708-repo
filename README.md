This data is from my pilot project for my masters. I was attempting to grow alfalfa plants, treating them with either 2 strains of Sinorhizobium meliloti 1021 or rm8530, or sterile media. 1021 only produces one type of EPS, whereas rm8530 produces 2 types. Half of the plants were watered normally and half were subjected to a drought period, after which all plants were recovered by routine watering. I have the final measurements after 7 weeks of growth, the height, dry root weight and dry shoot weight. I hope to observe which strain helped the plant tolerate drought stress more.

df <- as.data.frame(QMEE_data_set_example)

result <- aggregate(df$height_final, 
                    by = list(df$strain, df$condition), 
                    FUN = mean)
                    
