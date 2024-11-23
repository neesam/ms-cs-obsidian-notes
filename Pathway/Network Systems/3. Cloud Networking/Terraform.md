
### Overview

Terraform is an open-source Infrastructure as Code (IaC) tool developed by HashiCorp. It allows users to define, provision, and manage cloud infrastructure using declarative configuration files.

---

### Key Features
1. **Infrastructure as Code (IaC)**:
   - Infrastructure is defined in human-readable configuration files that can be version-controlled.
2. **Provider Support**:
   - Supports major cloud providers like AWS, Azure, Google Cloud, and on-premises solutions.
3. **Plan and Apply**:
   - Provides a detailed execution plan before making changes to the infrastructure.
4. **State Management**:
   - Maintains a state file to track resources and their configurations.
5. **Resource Graph**:
   - Automatically determines dependencies and resource creation order.

---

### Workflow
1. **Write**:
   - Define infrastructure in `.tf` files using the HashiCorp Configuration Language (HCL).
2. **Plan**:
   - Preview the changes Terraform will make using the `terraform plan` command.
3. **Apply**:
   - Execute the changes using `terraform apply` to create or update infrastructure.
4. **Destroy**:
   - Clean up resources using `terraform destroy` when no longer needed.

---

### Benefits
- Consistent and repeatable infrastructure deployments.
- Platform-agnostic, supporting multi-cloud and hybrid environments.
- Simplifies management of complex infrastructure with dependency tracking.
- Enables collaboration through version control of configuration files.

---

### Use Cases
- **Cloud Infrastructure Provisioning**:
   - Automate the creation of [[VPC|VPCs]], compute instances, and databases.
- **Multi-Cloud Management**:
   - Manage resources across AWS, Azure, and Google Cloud from a single tool.
- **Immutable Infrastructure**:
   - Rebuild and replace infrastructure instead of modifying in place.
- **Disaster Recovery**:
   - Quickly replicate infrastructure in different regions.

---

### Challenges
- Learning curve for HCL and understanding Terraform's state management.
- Potential for accidental resource changes if state is not carefully managed.
- Requires secure storage for sensitive state file information.

---

### Popular Commands
1. **`terraform init`**:
   - Initializes a new Terraform working directory.
2. **`terraform plan`**:
   - Shows the execution plan for infrastructure changes.
3. **`terraform apply`**:
   - Applies the planned changes to the infrastructure.
4. **`terraform destroy`**:
   - Deletes all resources defined in the configuration.

---

### Resources
- [Terraform Documentation](https://www.terraform.io/docs)
- [HashiCorp Learn Terraform](https://learn.hashicorp.com/terraform)
