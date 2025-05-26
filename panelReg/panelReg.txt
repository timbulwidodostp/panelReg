# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Fits Semiparametric Regression Models for Panel Count Survival Data Use panelReg (spef) With (In) R Software
install.packages("spef")
library("spef")
panelReg = read.csv("https://raw.githubusercontent.com/timbulwidodostp/panelReg/main/panelReg/panelReg.csv",sep = ";")
# Estimation Fits Semiparametric Regression Models for Panel Count Survival Data Use panelReg (spef) With (In) R Software
formula <- PanelSurv(id, time, count) ~ num + size + treatment
panelReg(formula, data = panelReg, method = "AEE", se = "Sandwich")
panelReg(formula, data = panelReg, method = "AEEX", se = "Impute", control = list(a = 0.1, R = 30))
panelReg(formula, data = panelReg, method = "MLs", se = "NULL")
panelReg(formula, data = panelReg, method = "EE.SWa", se = "Bootstrap", control = list(R = 30))
panelReg(formula, data = panelReg, method = "EE.HSWc", se = "Bootstrap", control = list(R = 30))
# Fits Semiparametric Regression Models for Panel Count Survival Data Use panelReg (spef) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished