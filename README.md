# DesignColor

Use beautiful color palettes for maximum 4 colors.

#example




library(devtools)



source_url("https://raw.github.com/student3841701/DesignColor/master/desco.R")



out <- data.frame(A=runif(16, 5.0, 7.5),B=runif(16, 2, 8),D=c("A","B","C","D","A","A","B","C","D","B","C","A","B","C","D","B"))


p   <- ggplot(out, aes(x=A, y=B,color=D)) + geom_point()


p +  scale_color_manual(values=desco("beachside"))


#reference from: https://digitalsynopsis.com/design/color-schemes-palettes-combinations/
