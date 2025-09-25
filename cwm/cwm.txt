# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Fit for the Cluster Weighted Model (CWM) Use cwm (flexCWM) With (In) R Software
install.packages("flexCWM")
library("flexCWM")
cwm = read.csv("https://raw.githubusercontent.com/timbulwidodostp/cwm/main/cwm/cwm.csv",sep = ";")
# Estimation Fit for the Cluster Weighted Model (CWM) Use cwm (flexCWM) With (In) R Software
attach(cwm)
str(cwm)
cwm <- cwm(WEIGHT ~ HEIGHT + HEIGHT.F , Xnorm = cbind(HEIGHT, HEIGHT.F), k = 2, initialization = "kmeans", modelXnorm = "EEE")
summary(cwm, concomitant = TRUE)
# Fit for the Cluster Weighted Model (CWM) Use cwm (flexCWM) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished