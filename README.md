# corelace-forex

rm(list=ls())
setwd ("C://TickDownloader//tickdata")

eurusd <- read.csv("EURUSD_M1_UTC+0_00_EURUSD11-12.2016.csv", header = FALSE)
eurusd <- data.frame(c)
eurusd$date <- eurusd$V1
eurusd$time <- eurusd$V2
eurusd$open <- eurusd$V3
eurusd$high <- eurusd$V4
eurusd$low <- eurusd$V5
eurusd$close <- eurusd$V6
eurusd$volume <- eurusd$V7

eurusd <- subset( eurusd, select = -c( V1 : V7 ))
eurgbp <- read.csv("EURGBP_M1_UTC+0_00_EURUSD11-12.2016.csv", header = FALSE)
eurgbp$date <- eurgbp$V1
eurgbp$time <- eurgbp$V2
eurgbp$open <- eurgbp$V3
eurgbp$high <- eurgbp$V4
eurgbp$low <- eurgbp$V5
eurgbp$close <- eurgbp$V6
eurgbp$volume <- eurgbp$V7
eurgbp <- subset( eurgbp, select = -c( V1 : V7 ))
