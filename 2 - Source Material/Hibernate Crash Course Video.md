Source: https://www.youtube.com/watch?v=xHminZ9Dxm4&t=683s

Tags: [[Java]], [[Hibernate]], 

Hibernate at its core solves a simple problem, crud operations between both the source code (e.g. entities in java, i.e. a person class and its attributes) and the actual database table and it's rows and columns (e.g. mysql, postresql, etc.) 


## How to add Hibernate dependency to project 

- go to build tool config file (pom.xml for maven, or build.gradle for gradle)
- Dependency:

```
<dependency>
	<groupId>org.hibernate</groupId>
	<artifactId>hibernate-core</artifactId>
	<version>6.1.2.Final</version>
</dependency>

```

- load changes from dependencies


## Annotation to map class to database table, attributed to rows 

@Entity - this marks the class as a database table 
@Table - Allows to insert fields for database table like "@Table(name = 'USERS')"


### Attribute annotations
- @Id - maps the primary key to attribute
- @GeneratedValue - auto increments, much more to it _________
- @Column - maps attribute to column (e.g. @Column(name = "birth_date"))


### Always create an empty constructors so Hibernate can create it's own empty columns when needed to

### [[Book Recommendation]]   
Java Persistence with Hibernate - 2nd Edition - Bauer, King, Gregory
Book tags: [[Java]], [[Hibernate]] 


### Hibernate offers a code template that lets a beginner create a project without having to do much

This template includes: 
#### SessionFactory class
- basically what hibernate is
#### setUp() function reads the 'hibernate.cfg.xml' file to config Hibernate


## Basic CRUD operations 

@Test - maps function to a test 

open session using a try/catch block:

```
@Test
void save_my_first_object_to_the_db() {

	User user = new User("Lisa", LocalDate.now()); //Create 

	try (Session session = sessionFactory.openSession()) {
		session.beginTransaction(); // good practice to do this 

		session.persist(user);

		sesion.getTransaction().commit();
	}
}
```