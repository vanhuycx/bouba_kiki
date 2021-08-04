
rds_files <- list.files("~/ShinyApps/bouba_kiki_jd/output/results",
                        pattern = "\\.rds$",
                        full.names = TRUE)

rds_files
data <- readRDS(rds_files[1])

data

participant_ID <- data$results$`sp_id`[[1]]
main_data <- data$results$`Main page`[[1]]


df <- read.table(text = main_data, sep =",", header = TRUE, stringsAsFactors = FALSE)



nrow(df)

# Slice the first two rows - preload, instruction - to a different data frame
df1<- df[c(1:2),]


# Slice the rest rows to a df

df2 <- df[c(3:nrow(df)),]


df1
nrow(df1)

df2
nrow(df2)

#data <- readRDS("~/ShinyApps/bouba_kiki_jd/output/results/id=4&p_id=2367fc1096a853bf332474de6264b918d432becd6d20240e7016086ec7c8f4fb&save_id=1&pilot=false&complete=true.rds")