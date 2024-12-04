Parent project: [OwnLab](https://github.com/orgs/HJHPio/projects/2)  
![OwnLabLogo](./IMGs/OwnLab/OwnLab-Logo-1_V2024.11.28.png)
# POGSearch
POGSearch began as a focused solution for indexing repositories from private GitLab instances, enabling comprehensive text searches across multiple repositories, branches, and commits. This approach allows users to find specific code snippets with a single query, eliminating the need to manually search each project. As the project has evolved, it has expanded to indexing also GitHub repositories.

## Quick Setup Guide (work in progress)
<!-- TODO: Update with Confizard integration and utility container for Terraform automation -->
The source code is currently being audited to provide simple deployment and maintenance options using OpenTofu (an open-source fork of Terraform).

## Description  
Project capabilities and used technologies:  
- **Keycloak Authentication**: Ensures secure access, requiring successful login for user participation.
- **Vue.js Frontend**: A minimalist interface offering robust search functionalities and administrative tools.
  - **Admin Tools**:
    - Create roles with designated index patterns to control user access levels to specific data sets.
    - Add users and assign roles for controlled access.
    - Import repositories using repository links.
  - **Researcher Tools**:
    - Conduct full-text searches with customized index patterns and queries.
    - Direct links to files within search results for quick access.
- **Docker Integration**: The entire system is encapsulated within a Docker Compose stack for seamless deployment and scalability.
- **Java Spring Boot API**: Facilitates backend operations, enhancing user interaction and data management.
- **OpenSearch**: Powers the search engine, offering scalable and effective search capabilities across vast datasets.
- **Bulk Import**: Admins can index multiple repositories at once by providing an API URL, for example, to request projects within a group from GitLab, along with an access token if the group is private.
- **Scheduled Updates**: Admins can schedule updates for indices.

## Video Preview
[![POGSearch Video Preview](https://github.com/Nailu776/POGSearch/assets/85428822/9f7a4414-246e-40fb-93ef-57500ff1ae9c)](https://drive.google.com/file/d/1Oun37QBJsSNsG4jkFyimEzPp0uTqweAJ/view?usp=sharing)

## Roadmap
[ROADMAP.md](./ROADMAP.md) file includes upcoming features and future plans.

## Changelog
[CHANGELOG.md](./CHANGELOG.md) file includes project changes in each release.

## Support
Everyone is welcome to submit an issue ticket on either GitHub or GitLab (depending on which platform this mirror of the project is hosted). Submitted issues will be automatically reviewed, and the main developer will be notified.
If you prefer private support (e.g., if you do not wish to share logs publicly), you can contact the project main developer via email at [support@hjhp.io](mailto:support@hjhp.io).

## Security
If you identify any security problems, please contact us immediately with the necessary details via email at [security@hjhp.io](mailto:security@hjhp.io).  
Please note that the email could end up in the spam folder. If you do not receive a timely response, please try emailing again.  
If the detected vulnerability is critical and the response to emails is not fast enough, please create an issue ticket to inform others and mitigate potential risks.
For more information please refer to [SECURITY.md](./SECURITY.md) file.

## Contributing
Everyone is welcome to contribute via GitHub pull requests or GitLab merge requests.
After reviewing and merging into the respective branches (*github-main* / *gitlab-main*), the final version of the software will be merged into the main branch on the private Git instance, and then all existing mirrors will be updated.  
Instructions on how to contribute can be found in [CONTRIBUTING.md](./CONTRIBUTING.md) file.

## Attribution
This project is maintained by its contributors.
The main tools and technologies used are listed in the [ATTRIBUTION-manual.md](./ATTRIBUTION-manual.md) file.
Automatically detected dependencies and their acknowledgments are listed in the [ATTRIBUTION.md](./ATTRIBUTION.md). file.

## License
*TL;DR:* This project is licensed under the MIT License.  
Everyone is welcome to fork and use it for private and commercial purposes.  
Full license can be found in [LICENSE](./LICENSE) file.  

## Project status
The project is in its initial state.  
The scope and targets may change after discussions in issues.
