# ravendb-project
IST769 Final Project

Pull the repo down locally:<br>
```git clone https://github.com/caseymwalsh/ravendb-project.git```

Load the Ravendb image:<br>
```docker-compose up -d ravendb```

RavenDB Studio Instructions:<br>

![image](https://user-images.githubusercontent.com/99757751/236104132-c5461259-07d2-45ac-b1bf-a57a9d90dac4.png)

Press "Create Database", create a database called "bookshelf"<br>
![image](https://user-images.githubusercontent.com/99757751/236104208-481bb62f-d372-4454-a8e5-5050bc0bf112.png)
![image](https://user-images.githubusercontent.com/99757751/236104450-8501e164-1617-4aa1-9d72-e9d82647fe7f.png)

Along the left side of the screen press "Tasks", then "Import Data"<br>
![image](https://user-images.githubusercontent.com/99757751/236104312-54744384-2bbb-4e85-b074-828eafcd1352.png)

Select "From CSV File", browse for the file, press "Import Collection". Note that the collection will be automatically named by the file name, but a different name can be specified in the "Import to Collection" field<br>
![image](https://user-images.githubusercontent.com/99757751/236104813-64668fd5-caf9-4553-88f1-af7feffe3e20.png)
![image](https://user-images.githubusercontent.com/99757751/236104839-23879b1b-4199-432b-aea9-d52787af7321.png)

Along the left side of the screen press "Indexes", then "Query"<br>
![image](https://user-images.githubusercontent.com/99757751/236365931-bf572455-d16c-4238-af15-9565da4af701.png)

Basic RQL query examples: RQL is written in the order that the query is run by the server (starting with from), unlike SQL.<br>

![image](https://user-images.githubusercontent.com/99757751/236364522-49636050-566e-40be-b05f-0128a44b269d.png)
![image](https://user-images.githubusercontent.com/99757751/236365809-7508f53a-0e2a-4596-bd61-86a117095afa.png)


RQL boost example: Boost changes the order in which results are returned. In the example below documents are filtered to those that contain the words "galaxy" or "sword", and then returned in descending order of the boost weight.<br>

![image](https://user-images.githubusercontent.com/99757751/236367130-c9be290d-9445-4b5f-b9a3-5786196f4c24.png)
