# Part 2: Cloud Architecture Considerations

***Rethinking the Type of Constituents Your Cloud Serves***

**Cloud Consumers**: These are the users of cloud services, like developers using public cloud resources. They focus on choosing the right services for their needs and integrating them effectively. 
                      They don't need to worry about the underlying infrastructure.

**Direct Customers**: These are the end users of services built on the cloud. They interact directly with the service and might not even know it's cloud-based.

**Cloud Service Providers**: These are the creators of cloud environments. They can be commercial vendors selling to the public or internal providers within a company serving employees or partners. 
                              They build and manage the cloud infrastructure and applications.

**Responsibilities based on Role**:


**Cloud Consumer**: Focuses on selecting and integrating services, avoiding isolated systems.
                    Containerization and microservices aid in managing these services.

**Cloud Service Provider**: Spends more time designing the cloud environment and building applications optimized for it. 
                            Consistency and long-term support are crucial for their services. They create an ecosystem for easy collaboration with partners.

                            NIST Cloud Reference Model:

This model by NIST (National Institute of Standards and Technology) illustrates the relationships between various cloud services to fulfill business needs.

**Cloud Consumers**:

These are the users of cloud services, internal or external.
Management tools ensure easy service access to meet evolving business needs.
This category includes applications, middleware, infrastructure, and on-premise services integrated with the cloud.
Cloud auditors (internal or external) oversee consumer adherence to obligations.

**Cloud Service Providers (CSPs)**:

These can be commercial companies or internal providers within an organization.
CSPs offer underlying physical and virtual resources to run cloud services.
They might also develop applications and business services specifically for the cloud environment.

**Interconnectedness and Management**:

All cloud models are interconnected and supported by a partner ecosystem.
CSPs provide a unified architecture for consistent service support and management.
Management platforms are crucial for service operation, performance monitoring, and business alignment.

**Service Orchestration**:

CSPs must support all major cloud models (private, public, hybrid, etc.).
Service orchestration is essential to prevent isolated silos and ensure services work together seamlessly.

**Overall Management**:

Effective cloud management requires services for:

Supporting business needs
Managing configurations
Providing on-demand resource allocation
Enabling interoperability and service portability (moving services between cloud providers)
In simpler terms, the cloud architecture involves various components working together. Consumers use services, providers manage and deliver them, and everything is interconnected for smooth operation. 
Effective management ensures services align with business needs and function efficiently.

***Planning for Deployment***

Hybrid cloud isn't a single model, but a combination of various services on different platforms.
Defining the architecture focuses on how these services interact, not creating a unified system.
Cloud management tools are crucial for the hybrid cloud architecture.

**Challenges of Hybrid Cloud Architecture**:

Services are distributed and not combined into one system.
Understanding relationships between these distributed services is critical.
Best practices involve creating templates to link services effectively.

**Important Considerations**:

Track service functions, usage rules, definitions, and dependencies.
Plan for how the environment behaves under various conditions (adding services, new partners).
Design for change and adaptability (adding new cloud services, business partners).

**1. Latency and Performance**

**Challenges and Considerations**:

Monitor and measure entire environment for optimal performance.
Latency is a major concern impacting customer experience (order confirmation speed etc.).
Critical applications requiring low latency might be better suited for private cloud or on-premises solutions (transaction management).
Complex data manipulation tasks might benefit from on-premises or private cloud solutions.

**Making Informed Decisions**:

Public cloud SaaS applications might be suitable for tasks with acceptable latency (customer management, HR).
Service location matters - geographically distant services can cause latency issues.
Understand service interactions - plan based on how services need to work together.
Public vs. private cloud choice depends on the specific service and customer needs.

**Planning for Flexibility**:

Build flexibility into the plan to address varying latency requirements.
Public cloud can be cost-effective for collaborative workspaces (depending on collaboration type).
Mission-critical transactions require optimized performance (private cloud).
Low data volume tasks are suitable for public cloud.

**Composite Services and Adaptability**:

Consider combining services to create composite services with varying latency needs.
Leverage public cloud for cost-effective functionalities within a secure private cloud environment.
Be prepared to relocate services based on changing performance needs (data volume increase etc.).

**Microservices and Containers for Reduced Latency**:

Tightly couple microservices in containers for low-latency execution.
Well-defined APIs and orchestration services improve performance control.
Leverage caching mechanisms to minimize latency when relying on external services.

A well-architected hybrid cloud based on best practices ensures smooth operation.
