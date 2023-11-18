# learnInPublic
Day to Day / Weekend to Weekend Learning doc

## EnableJpaAuditing
1. @EnableJpaAuditing Annotaion in Spring framework - can be used optionally to enable auditing of JPA entity.
2. @EnableJpaAuditing is to automatically populate certain fields in JPA entities, such as created by, creation date, last modified by, and last modification date.
3. Use in Main Class of Spring Boot App.
4. Example:

   ` @CreatedBy
    private String createdBy;

    @CreatedDate
    private LocalDateTime createdAt;

    @LastModifiedBy
    private String lastModifiedBy;

    @LastModifiedDate
    private LocalDateTime lastModifiedAt; `

   Insted of:
   
  ` public void setCreatedBy(String createdBy) {
        this.createdBy = createdBy;
    }
    
    public void setCreatedAt(LocalDateTime createdAt) {
        this.createdAt = createdAt;
    }

    public void setLastModifiedBy(String lastModifiedBy) {
        this.lastModifiedBy = lastModifiedBy;
    }

    public void setLastModifiedAt(LocalDateTime lastModifiedAt) {
        this.lastModifiedAt = lastModifiedAt;
    }

    // You'll need to call these methods appropriately when creating or updating entities
} `

## Solr

Why Use Solr Alongside JPA:
Enhanced Search Capabilities: Solr provides advanced search features, including full-text search, faceted search, and geospatial search. If your application requires sophisticated search functionality, integrating Solr can significantly enhance the user experience.

Diverse Data Sources: Solr is not limited to relational databases. It can index data from various sources, including JSON, XML, and CSV. This flexibility is beneficial when dealing with diverse data formats.

Scalability and Performance: Solr is designed for high scalability and performance in search operations. If your application needs to handle large volumes of data and perform complex searches, Solr can be a valuable addition.

Separation of Concerns: JPA focuses on persisting and retrieving structured data from relational databases, while Solr focuses on providing efficient search capabilities. Combining the two allows each component to excel in its specialized domain.

## React.Fragment

React.Fragment is a built-in component in React that provides a way to group multiple elements together without adding an extra node to the DOM.

In JSX, when you return multiple elements from a component, they must be enclosed in a single parent element
