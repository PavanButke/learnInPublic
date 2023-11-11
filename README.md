# learnInPublic
Day to Day / Weekend to Weekend Learning doc

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
