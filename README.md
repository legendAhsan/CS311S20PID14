# CS311S20PID14
Development Team of Activity Scheduling Project.
TimeTableGenerator(CD[][][], as[45],) 
{
	
	FTT[][as.length]
	Teachers[][45];
	for class in dim1 of classDetails
		ln=1;
		int TCH =0;
		for(int i=0; i<CD[class].lengthofdim2; i++)
		{
			TCH +=CD[class][i][4];
		}
		while(TCH>1)
			For each teacher in dim2 of classDetails[class]
				teacherno=cd[class][teacher][2];
				if(as[ln=0])
				{
					ln++;
				}
				else if(teachers[teacherno][ln]==NULL && cd[class][teacher][4]!=0 && cd[class][teacher][5]=0)
				{
					FTT[class][ln]==cd[class][teacher][1]+cd[class][teacher][3];
					teachers[teacherno][ln]=class+cd[class][teacher][3];
					cd[class][teacher][4]--;
					TCH--;
					ln++;
				}
				else if(cd[class][teacher][5]=1 && cd[class][teacher][4]!=0 )
				{
					allow=1;
					for(i=ln; i<(ln+cd[class][teacher][4]); i++)
					{
						if(teacher[teacherno][i]==!NULL or as[i]!==1)
						{
							allow=0;
							break;
						}
					}
					if(allow)
					{
								for(i=ln; i<(ln+cd[class][teacher][4]); i++)
								{
									FTT[class][i]==cd[class][teacher][1]+cd[class][teacher][3];
									teacher[teacherno][i]=class+cd[class][teacher][3];
									cd[class][teacher][4]--;
									TCH--;
									ln++;
								}
					}
					
				}	
}		
minimumRoomAllocator(FTT[class][as[length]]
{
	
}
