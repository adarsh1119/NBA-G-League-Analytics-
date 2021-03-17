# NBA-G-League-Analytics-

#****4

#-Matrices

#-FieldGoalAttempts

#-FieldGoal

#-Games

#-Minutes Played

#-Salary

#-Vectors

#-Players

#-Seasons



#-Comments


#****Seasons

Seasons<-c("2005","2006","2007","2008","2009","2010","2011","2012","2013","2014")
Seasons

#****Players

Players<-c("KobeBryant","JoeJohnson","leBronJames","CarmeloAnthony",
           "DwightHoward","ChirsBosh","ChrisPaul","KevinDurant",
           "DerrickRose","DwayneWade")

#****Salaries

KobeBryant_Salary<-c(15946875,17718750,19490625,21262500,23034375,
                     24806250,25244493,27849149,30453805,23500000)
KobeBryant_Salary


JoeJohnson_Salary<-c(12000000,12744189,13488377,14232567,14976754,
                     16324500,18038573,19752645,21466718,23180790)
JoeJohnson_Salary


LeBronJames_Salary<-c(4621800,8528090,13041250,14410581,15779912,
                      14500000,16022500,17545000,19067500,20644400)
LeBronJames_Salary


CarmeloAnthony_Salary<-c(3713640,4694041,13041250,14410581,15779912,
                      17149243,18518574,19450000,22407474,22458000)
CarmeloAnthony_Salary


DwightHoward_Salary<-c(4493160,4806720,6061274,13758000,15202590,
                       16647180,18091770,19536360,20513178,21436271)
DwightHoward_Salary


ChrisBosh_Salary<-c(3348000,12455000,14410581,15779912,
                    14500000,16022500,17545000,19067500,20644400)
ChrisBosh_Salary


ChrisPaul_Salary<-c(3144240,3380160,3615960,4574189,13520500,
                   14940153,16359805,17779458,18668431,20068563)
ChrisPaul_Salary


KevinDurant_Salary<-c(0,0,41712000,4484040,4796880,6053663,
                      15506632,1666930,17832627,18995624)
KevinDurant_Salary


DerrickRose_Salary<-c(0,0,0,4822800,5184480,5546160,
                      6993708,16402500,18862875)
DerrickRose_Salary


DwayneWade_Salary<-c(3031920,3841443,13041250,14410581,
                     15779912,14200000,15691000,17182000,18673000,15000000)
DwayneWade_Salary

#Matrix


Salary<-rbind(KobeBryant_Salary,JoeJohnson_Salary,LeBronJames_Salary,CarmeloAnthony_Salary,DwightHoward_Salary,ChrisBosh_Salary,ChrisPaul_Salary,KevinDurant_Salary,DerrickRose_Salary,DwayneWade_Salary)


Salary

#str(Salary)

View(Salary)

colnames(Salary)

head(Salary,3)


colnames(Salary)<-Seasons

head(Salary)


Salary

rownames(Salary)


head(Salary)

rownames(Salary)<-Players

head(Salary)


View(Salary)

#Games

KobeBryant_G<-c(80,77,82,82,73,82,58,78,6,35)

JoeJohnson_G<-c(82,57,82,79,76,72,60,72,79,80)

LeBronJames_G<-c(79,78,75,81,76,79,62,76,77,69)

CarmeloAnthony_G<-c(80,65,77,66,69,77,55,67,77,40)

DwightHoward_G<-c(82,82,82,79,82,78,54,76,71,41)

ChrisBosh_G<-c(70,69,67,77,70,77,57,74,79,44)

ChrisPaul_G<-c(78,64,80,78,45,80,60,70,62.82)

KevinDurant_G<-c(35,35,80,74,82,78,66,81,81,27)

DerrickRose_G<-c(40,40,40,81,78,81,39,0,10,51)

DwayneWade_G<-c(75,51,51,79,77,76,49,69,54,62)

#Matrix

Games<-rbind(KobeBryant_G,JoeJohnson_G,LeBronJames_G,CarmeloAnthony_G,DwightHoward_G,ChrisBosh_G,ChrisPaul_G,KevinDurant_G,DerrickRose_G,DwayneWade_G)

Games


colnames(Games)<-Seasons

Games

rownames(Games)<-Players

Games

head(Games)

head(Games,3)

tail(Games,3)

Games[3,8]

Games["leBronJames","2012"]

#Minutes Played

KobeBryant_MP<-c(3277,3140,3192,2960,2835,2779,2232,3013,177,1207)

JoeJohnson_MP<-c(3340,2359,3343,3124,2886,2554,2127,2642,2575,2791)

LeBronJames_MP<-c(3361,3190,3027,3054,2966,3063,2326,2877,2903,2493)

CarmeloAnthony_MP<-c(2941,2486,2806,2277,2634,2751,1876,2482,2982,1428)

DwightHoward_MP<-c(3021,3023,3088,2821,2843,2935,2070,2722,2396,1223)

ChrisBosh_MP<-c(2751,2658,2425,2928,2526,2795,2007,2454,2531,1556)

ChrisPaul_MP<-c(2808,2353,3006,1712,2880,2181,2335,2171,2857)

KevinDurant_MP<-c(1255,1255,2768,2885,3239,3038,2546,3119,3122,913)

DerrickRose_MP<-c(1168,1168,1168,3000,2871,3026,1375,0,311,1530)

DwayneWade_Mp<-c(2892,1931,1954,3048,2792,2823,1625,2391,1775,1971)

#Matrix

MinutesPlayed<-rbind(KobeBryant_MP,JoeJohnson_MP,LeBronJames_MP,CarmeloAnthony_MP,DwightHoward_MP,ChrisBosh_MP,ChrisPaul_MP,KevinDurant_MP,DerrickRose_MP,DwayneWade_Mp)

MinutesPlayed

colnames(MinutesPlayed)<-Seasons
rownames(MinutesPlayed)<-Players

MinutesPlayed
Games

round(MinutesPlayed/Games)


#Field Goals

KobeBryant_FG<-c(978,813,775,800,716,740,574,738,31,266)

JoeJohnson_FG<-c(632,536,647,620,635,514,423,445,462,446)

LeBronJames_FG<-c(875,772,794,789,768,758,621,765,767,624)

CarmeloAnthony_FG<-c(756,691,728,535,688,684,44,669,743,358)

DwightHoward_FG<-c(468,526,583,560,510,619,416,470,473,251)

ChrisBosh_FG<-c(549,543,507,615,600,524,393,485,492,343)

ChrisPaul_FG<-c(407.381,630,631,314,430,425,412,406,568)

KevinDurant_FG<-c(306,306,587,661,794,711,634,731,849,238)

DerrickRose_FG<-c(208,208,208,574,672,711,302,0,58,338)

DwayneWade_FG<-c(699,472,439,854,719,692,416,569,415,509)

#Matrix


FieldGoals<-rbind(KobeBryant_FG,JoeJohnson_FG,LeBronJames_FG,CarmeloAnthony_FG,DwightHoward_FG,ChrisBosh_FG,ChrisPaul_FG,KevinDurant_FG,DerrickRose_FG,DwayneWade_FG)

#rm(KobeBryant_FG,JoeJohnson_FG,LeBronJames_FG,CarmeloAnthony_FG,
#DwightHoward_FG,ChrisBosh_FG,ChrisPaul_FG,KevinDurant_FG,
#DerrickRose_FG,DwayneWade_FG)

colnames(FieldGoals)<-Seasons

rownames(FieldGoals)<-Players

FieldGoals

Games

round(FieldGoals/Games)

round(FieldGoals/Games,1)

#Field Goals Attempts

KobeBryant_FGA<-c(2173,1757,1690,1712,1569,1639,1336,1595,73,713)

JoeJohnson_FGA<-c(1395,1139,1497,1420,1386,1161,931,1052,1018,1025)

LeBronJames_FGA<-c(1823,1621,1642,1613,1528,1485,1169,1354,1353,1279)

CarmeloAnthony_FGA<-c(1572,1453,1481,1207,1502,1503,1025,1489,1643,806)

DwightHoward_FGA<-c(881,873,974,979,834,1044,726,813,800,423)

ChrisBosh_FGA<-c(1087,1094,1027,1263,1158,1056,807,907,953,745)

ChrisPaul_FGA<-c(947,871,1291,1255,637,928,890,856,870,1170)

KevinDurant_FGA<-c(647,647,1366,1390,1668,1538,1297,1433,1688,467)

DerrickRose_FGA<-c(436,436,436,1208,1373,1597,695,0,164,835)

DwayneWade_FGA<-c(1413,962,937,1739,1511,1384,837,1093,761,1084)


#Matrix

FieldGoalAttempts<-rbind(KobeBryant_FGA,
                         JoeJohnson_FGA,
                          LeBronJames_FGA,
                           CarmeloAnthony_FGA,
                            DwightHoward_FGA,
                             ChrisBosh_FGA,
                              ChrisPaul_FGA,
                               KevinDurant_FGA,
                                DerrickRose_FGA,
                                 DwayneWade_FGA)


#rm(KobeBryant_FGA,JoeJohnson_FGA,LeBronJames_FGA,CarmeloAnthony_FGA,DwightHoward_FGA,ChrisBosh_FGA,ChrisPaul_FGA,KevinDurant_FGA,DerrickRose_FGA,DwayneWade_FGA)

colnames(FieldGoalAttempts)<-Seasons
rownames(FieldGoalAttempts)<-Players


#Points


KobeBryant_PTS<-c(2832,2430,2323,2201,1970,2078,1616,2133,83,782)

JoeJohnson_PTS<-c(1653,1426,1779,1688,1619,1312,1129,1170,1245,1154)

LeBronJames_PTS<-c(2478,2132,2250,2304,2258,2111,1683,2036,2089,1743)

CarmeloAnthony_PTS<-c(2122,1881,1978,1504,1943,1970,1245,1920,2112,966)

DwightHoward_PTS<-c(1292,1443,1695,1624,1503,1784,1113,1296,1297,646)

ChrisBosh_PTS<-c(1572,1561,1496,1746,1678,1438,1025,1232,1281,928)

ChrisPaul_PTS<-c(1258,1104,1684,1781,841,1268,1189,1186,1185,1564)

KevinDurant_PTS<-c(903,903,1624,1871,2472,2161,1850,2280,2593,686)

DerrickRose_PTS<-c(597,597,597,1361,1619,2026,852,12,159,904)

DwayneWade_PTS<-c(2040,1397,1254,2386,2045,1941,1082,1463,1028,1331)

#Matrix

Points<-rbind(KobeBryant_PTS,JoeJohnson_PTS,LeBronJames_PTS,CarmeloAnthony_PTS,
              DwightHoward_PTS,ChrisBosh_PTS,ChrisPaul_PTS,KevinDurant_PTS,
              DerrickRose_PTS,DwayneWade_PTS)

#rm(KobeBryant_PTS,JoeJohnson_PTS,LeBronJames_PTS,CarmeloAnthony_PTS,DwightHoward_PTS,ChrisBosh_PTS,ChrisPaul_PTS,KevinDurant_PTS,DerrickRose_PTS,DwayneWade_PTS)

colnames(Points)<-Seasons

rownames(Points)<-Players

Points

?matplot

FieldGoals

matplot(FieldGoals)

t(FieldGoals)

matplot(t(FieldGoals))

Salary

matplot(t(Salary),type="b",pch=15:18,col=c(1:4,6))

matplot(t(FieldGoals),type="b",pch=15:18,col=c(1:4,6))

#***5


FieldGoals

Games

matplot(t(FieldGoals/Games),type="b",pch=15:18,col=c(1:4,6))


matplot(t(FieldGoals),type="b",col=c(1:4,6))

matplot(t(FieldGoals),type="b",pch=15:18,col=c(1:4,6))

matplot(t(Games),type="b",pch=15:18,col=c(1:4,6))

legend("bottomleft",inset=0.2,legend=Players,col=c(1:4,6),horiz=F,pch=15:18)

?legend

#Normalize the data

FieldGoals/Games

t(FieldGoals/Games)

matplot(t(FieldGoals/Games),type="b",pch=15:18,col=c(1:4,6))

legend("bottomleft",inset=0.01,legend=Players,col=c(1:4,6),horiz=F,pch=15:18)

#Notice Dereck

#A

t(FieldGoals/FieldGoalAttempts)

matplot(t(FieldGoals/FieldGoalAttempts),type="b",pch=15:18,col=c(1:4,6))

legend("bottomleft",inset=0.01,legend=Players,col=c(1:4,6),horiz=F,pch=15:18)

#legend("bottomleft",inset=0.01,legend=Players,col=c(1:4,6),horiz=F)
#Notice Kobes acc is going down
#and Dwight Howard is prettt consistent
#v can also look at MinutesPlayed/Games
# or Salary/Games

#***6

#Subsetting

x<-c("a","b","c","d","e")

x

x[c(1,5)]

x[1]

Games

Games[1:3,6:10] #Games[c(1,2,3),c(6:10)]

Games[c(1,10),]

Games[,c("2008","2009")] #Error in Games: subscript out of bounds

Games[1,]

is.matrix(Games[1,])

is.vector(Games[1,])

Games[1,]

Games[1,drop=F]

is.matrix(Games[1,,drop=F])

is.vector(Games[1,,drop=F])

Games[1,1,drop=F]

Games[1,1]

Games[1,]

Games[c(1,10),]

is.matrix(Games[c(1,10),])

Games[1,5]

is.matrix(Games[1,5])

Games[1,5]

Games[1,5,drop=F]

#Visualizing Subsets

#Mins played for the last 10 yrs of all players

MinutesPlayed

matplot(t(MinutesPlayed),type="b",pch=15:18,col=c(1:4,6))

legend("bottomleft",inset=0.01,legend=Players,col=c(1:4,6),horiz=F,pch=15:18)

Points

matplot(t(Points),type="b",pch=15:18,col=c(1:4,6))

FieldGoals

matplot(t(FieldGoals),type="b",pch=15:18,col=c(1:4,6))

#legend("bottomleft",inset=0.01,legend=Players,col=c(1:4,6),horiz=F)

#get the top 3 players

Data<-MinutesPlayed[1:3,]

Data

View(Data)

MinutesPlayed

matplot(t(MinutesPlayed[1:3,]),type="b",pch=15:18,col=c(1:4,6))

legend("bottomleft",inset=0.01,legend=Players[1:3],col=c(1:4,6),horiz=F,pch = 15:18)

#Only KB

Data<-MinutesPlayed[1,]
Data

matplot(t(Data),type="b",pch=15:18,col=c(1:4,6))

legend("bottomleft",inset=0.01,legend=Players[1],col=c(1:4,6),horiz=F,pch=15:18)

MinutesPlayed[1,]

MinutesPlayed[1,,drop=F]

Data<-MinutesPlayed[1,,drop=F]

matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))

legend("bottomleft",legend = Players[1],col = c(1:4,6),horiz = F,pch = 15:18)

#***7

? matplot


Data<-MinutesPlayed[1,,drop=F]

matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))

legend("bottomleft",inset=0.01,legend = Players[1],col = c(1:4,6),horiz = F)

#what does the dip indicate

Data<-Points[1,,drop=F]

matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))

legend("bottomleft",inset=0.01,legend = Players[1],col = c(1:4,6),horiz = F,pch = 15:18)



Data<-Salary[1,,drop=F]

matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))

legend("bottomleft",inset=0.01,legend = Players[1],col = c(1:4,6),horiz = F)


Data<-MinutesPlayed[2,,drop=F]

matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))

legend("bottomleft",inset=0.01,legend = Players[2],col = c(1:4,6),horiz = F)


Data<-Points[2,,drop=F]

matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))

legend("bottomleft",inset=0.01,legend = Players[2],col = c(1:4,6),horiz = F,pch = 15:18)





Data<-Salary[2,,drop=F]

matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))

legend("bottomleft",inset=0.01,legend = Players[2],col = c(1:4,6),horiz = F,pch = 15:18)













# Step 1: Function(){}
# Step2:

function(){
        
  Data<-MinutesPlayed[1,,drop=F]
  
  matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))
  
  legend("bottomleft",inset=0.01,legend = Players[1],col = c(1:4,6),horiz = F,pch = 15:18)
  
  
}



# step3:

myplot<-function() { 
      Data<-MinutesPlayed[1,,drop=F]
      
      matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))
      
      legend("bottomleft",inset=0.01,legend = Players[2],col = c( 1:4,6),horiz = f)
      
  
  
}
  
myplot()


myplot<-function(){
  
  Data<-MinutesPlayed[3,,drop=F]
  
  matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))
  
  legend("bottomleft",inset=0.01,legend = Players[3],col = c(1:4,6),horiz = F,pch = 15:18)
  
  
}

myplot()


myplot<-function(){
  
  Data<-MinutesPlayed[c(2,9),,drop=F]
  
  matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))
  
  legend("bottomleft",inset=0.01,legend = Players[2:3],col = c(1:4,6),horiz = F,pch = 15:18)
  
  
}

myplot()



myplot<-function(){
  
  Data<-MinutesPlayed[1:5,,drop=F]
  
  matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))
  
  legend("bottomleft",inset=0.01,legend = Players[1:5],col = c(1:4,6),horiz = F,pch = 15:18)
  
  
}

myplot()


myplot<-function(rows){
  
  
  Data<-MinutesPlayed[rows,,drop=F]
  
  matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))
  
  legend("bottomleft",inset=0.01,legend = Players[rows],col = c(1:4,6),horiz = F,pch = 15:18)
  
  
}

myplot()




myplot

myplot(1:3)

myplot(1:5)

myplot(c(1,5,10))



myplot<-function(rows){
  
  
  Data<-Games[rows,,drop=F]
  
  matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))
  
  legend("bottomleft",inset=0.01,legend = Players[rows],col = c(1:4,6),horiz = F,pch = 15:18)
  
  
}

myplot(1:3)



myplot<-function(rows){
  
  
  Data<-FieldGoals[rows,,drop=F]
  
  matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))
  
  legend("bottomleft",inset=0.01,legend = Players[rows],col = c(1:4,6),horiz = F,pch = 15:18)
  
  
}

myplot(1:3)


myplot<-function(rows){
  
  
  Data<-Salary[rows,,drop=F]
  
  matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))
  
  legend("bottomleft",inset=0.01,legend = Players[rows],col = c(1:4,6),horiz = F,pch = 15:18)
  
  
}

myplot(1:3)

#****8


myplot<-function(data,rows){
  
  
  Data<-data[rows,,drop=F]
  
  matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6))
  
  legend("bottomleft",inset=0.01,legend = Players[rows],col = c(1:4,6),horiz = F,pch = 15:18)
  
  
}

myplot(Salary,1:3)

myplot(Games,1:3)

myplot(FieldGoals,1:3)

myplot(FieldGoals/Games,1:2)

myplot(FieldGoals,1)

myplot(Salary,c(1,5,7))



myplot<-function(data,rows=1:10){
  
  
  Data<-data[rows,,drop=F] # this is subsetting the data
  
  matplot(t(Data),type = "b",pch=15:18,col = c(1:4,6)) # v r plotting the data
  
  #legend("bottomleft",inset=0.01,legend = Players[rows],col = c(1:4,6),horiz = F,pch = 15:18)
  
  
}

myplot(Salary)

myplot(Salary,1:3)

myplot(Salary,c(1,3,9,10))

myplot(MinutesPlayed)

myplot(MinutesPlayed/Games)

myplot(MinutesPlayed/Games,3)

myplot(MinutesPlayed/Games,1:3)



# More  Insights

myplot(Salary)

# notice KB was always High

# His highest is record $30 Mill $/Yr

# Then v hv joe johnsos


myplot(Salary/Games)

#****   


# Notices there r a few anamolies

# notices KB & Der Rose r getting paid

# v high per games


myplot(Salary/FieldGoals)

# In games metrics

myplot(MinutesPlayed)
myplot(Points)

# notices DR & KB their pts dropped suddenly
# why 
# injury
# so v can normalize in game metrics 

myplot(FieldGoals/Games)

# this is showing howmany FGs hv been scored per game  


myplot(FieldGoals/FieldGoalAttempts)

# this is interesting 

# this is basically the accuracy of the player


myplot(FieldGoalAttempts/Games)

# this is the actual attempts per gm 
# this show how many actual attempts he makes per gm

# nd now if v look at this 


myplot(Points/Games)

# this means he doesnt score many pts per gm


# Interesting Obs

myplot(MinutesPlayed/Games)
# note here these r the top 10 player and the MP/G
# why 
# unexplained 

myplot(Games)
# if v look at this and try to und the prev pt


# time is valuable  

myplot(FieldGoals/MinutesPlayed)

# time is the most imp

# Player Style 

myplot(Points/FieldGoals)

# in BB v  can score a 2 pt or 3 ptr
