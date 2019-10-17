# MAVEN PROJECT SETUP FOR SPRING CORE APPLICATION 

---
## **```STEP 1:```**
1. **Open EclipseIDE** 
2. **Click on File**
   1. **Click on New**
      1. **Click on "_MAVEN PROJECT_"**

![ECLIPSE](https://github.com/ALL-GET-IN-TT/SPRING/blob/master/Snapshots/step1.png?raw=true "STEP1")

## **`STEP 2:`**
1. **Specify the Workspace location**
2. Check the option **_Add Project(s) To Working Set_**
3. Click On **Next**

![2WorkspaceLocation]()

## **`STEP 3:`**
1. Select _**archetype**_ with **maven-archetype-quickstart** as an **Artifact Id** value 
2. Click On **Next**.

![3maven-archetype]()

## **`STEP 4:`**
1. Specify **archetype parameters**
   1. **Group Id:** (The value is like a part of domain name) 
      - Generally Value starts with subdomain names like **com,net,org etc** followed by name of your choice.
      - Example : **_com.github_** 
    2. **Artifact Id:** (This will be your Project name)
       - Example: **springcore**
    3. **NOTE:** All letters of Artifact Id must be **_lower case_**.
    4. Now Click On **_Finish_**

![4ArchetypeParameter]()

## **`STEP 5:`**
1. Now change **Java JRE version**
   1. Open **_pom.xml_** file.
   2. copy the following XML code and paste inside XML **```<properties>```** tag.
```XML
<properties>
      <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
      <maven.compiler.source>1.8</maven.compiler.source>
      <maven.compiler.target>1.8</maven.compiler.target>
</properties>
```

![5PomXmlJavaVersion]()

2. Now do the **``MAVEN Update``**:
   - **Right click** on PROJECT.
   - Select **Maven ---> Update Project...**
   - Check the option for ``Force Update of Snapshots/Releases``
  

      ![5_2_ForceUpdateMaven]()


## **`STEP 6:`** 
# **``DEPENDENCIES``**
---

1. SPRING CORE [5.1.5 Release]
2. SPRING CONTEXT [5.1.5 Release]
- **Note: All dependencies must are of same release version.**
#  6.1 SPRING CORE
1. Navigate to the URL [mvnrepository.com](https://mvnrepository.com)
2. Search for the **spring core**
3. Select the required release **version** of spring core dependency (depending on the usage and release date)
- ![6_SpringCore_dependency]()
 
4. Copy the **maven** code and paste inside the ```<dependencies>``` tag of the _pom.xml_ file.
   - 
   


![6_SpringCore_dependency_Maven]()

#  6.2 SPRING CONTEXT
1. Navigate to the URL [mvnrepository.com](https://mvnrepository.com)
2. Search for the **spring context**
3. Select the required release **version** of spring context dependency.
4. Copy the **maven** code and paste inside the ```<dependencies>``` tag of the _pom.xml_ file.

![6_SpringCore_dependency_Maven]()

5. Now do MAVEN Update. ( Repeat Step 5.2 )
