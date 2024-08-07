# System Administration using Windows Server
(WINDOWS SERVER | WINDOWS | POWERSHELL | VMWARE WORKSTATION | VIRTUALIZATION)

Implemented a scalable network infrastructure in two different states (Headquarters in Luanda state and Branch in Benguela state) tailored to a company's business volume, ensuring flexibility and efficiency, and ensuring that branch users had the same working conditions and performance as head office users.

Configured the following services: AD DS, DNS, DFS, DHCP, FTP, IIS, Storage File Server, Failover Cluster, O and P Drive Server.

Requirements for Headquarters (Luanda state) and Branch (Benguela state) servers and switches:
- IP Address Configuration
- Server 1 (Windows Server 2019), Services Configuration: AD DS, DNS, DFS, Storage File Server, O and P Drive Server.
- Server 2 (Windows Server 2019), Services Configuration: DHCP, FTP, IIS, Failover Cluster.
- Clients (Windows 7, 8, or 10), Dynamic/Static IP Assignment from DHCP.
- Installation of BG Info on Server 1, Server 2 and Clients.

Configured services:
- Configured the Company Domain (Headquarters and Branch).
- Configured the OU in each site (Headquarters and Branch), with its own structure to store its objects.
- Configured department objects in the OU.
- Configured groups in the OU.
- Created user accounts to be able to log into Luanda and Benguela.
- Restricted access to the system in a certain period of the day and days of the week.
- Created administrator accounts (normal and administration) that have access to all servers and insertion in a group.
- Configured P:Drive for each user, to store automatically mapped personal data.
- Configured Dropbox with read and write permission to share data from all users.
- Restricted access to department folders allowing only members to have access to their department's folder, except DG members who have access to folders in all departments.
- Configured company websites available via IIS.
- Configured the company's FTP with access restricted to members of a group.

Security:
- Infrastructure security is managed in the OU via GPO for computers and users.

**AD DS Configuration**
<br>![00](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/976ae4e3-cfda-4538-9cea-66d943e53438)
<br>![01](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/ee4efad2-aed0-4f23-8802-5c70a60b0722)
<br>![02](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/4b52def1-a981-4445-8e4c-ab83c7180a96)
<br>![03](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/32507d53-8b08-4a56-aa8a-b4b078f557f6)
<br>![04](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/f72a4a33-0a8c-47c0-a089-aa720b5e5992)
<br>![05](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/7db25af0-9148-43b3-9e6f-2e8414c1f4b2)
<br>![06](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/89be1a3c-a0a8-46cc-a9dc-75aba50a6c9a)
<br>![07](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/62732c30-581b-4ab8-b106-62b869d80393)
<br>![08](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/0f48d86e-ca65-4ec6-9446-6caa05c0a4c8)
<br>![09](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/35ab266a-d92d-406b-91de-054b485a264d)
<br>![10](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/2e1cfb21-6dfa-49df-a959-96698d002833)
<br>![11](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/00c1ff65-4266-4602-948b-9f70e03569e9)
<br>![12](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/725b6c9e-1422-437a-9e81-f1e067a04727)
<br>![13](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/7e297c3b-5377-4fe8-a584-cd4cc04ee7b2)
<br>![14](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/eedde27d-c03c-431a-b9a0-800b8999463b)
<br>![15](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/84590e44-c3a0-4516-9ec8-5889cfe2ef33)
<br>![16](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/a9c1246f-52d6-4f89-a4ae-060ab40aeca7)
<br>![17](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/ee2d3434-3ccc-4a2c-9f2f-9ac386d4378f)
<br>![18](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/c164af00-1408-4ddc-88e3-b0029b9e8ef6)
<br>![19](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/cfb2b82b-1ca3-4f81-a0d3-fff0f3eceec0)
<br>![20](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/c7bd09cf-2d69-4e27-a5d5-1680195a0e69)
<br>![21](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/d2f3930f-3a91-4ede-909f-99acf63886c9)
<br>![22](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/3ffb59b8-a0f3-456a-98e3-a68fe6f9c6dd)
<br>![25](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/15ea26c6-124a-400a-ae66-7e1611bba867)
<br>![26](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/3eefe49b-7166-47b8-87d6-29c3019112c5)
<br>![27](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/c6353c1e-b9b2-474a-81ab-54f60397a0f8)

**DNS Configuration**
<br>![28](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/75a8de69-d432-4447-bf15-ba3e1e173559)
<br>![29](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/bbd7877c-5216-498a-a343-3163d3097e4a)
<br>![30](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/cebf5209-77a6-4ba0-b460-05ed422e341f)
<br>![31](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/8e7bf62d-ff66-47a3-a23f-de02b523e1c4)
<br>![32](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/ee2d77f8-34d8-4d20-805f-733cd5ea1526)
<br>![33](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/21fc0ed2-94b8-4353-90df-67fefce488b3)
<br>![34](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/a0f64eb5-0967-46b5-b5a2-7b8adc7e5f12)
<br>![35](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/0f3d1584-de50-47d2-8055-718f2538e6c4)
<br>![36](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/ebcb2dbc-94f0-4c90-8e98-ea3d56840c78)
<br>![37](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/7f4cafbe-8cf0-4b33-ae89-ee264d5ea058)
<br>![38](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/ae24ba8c-a0d4-47cf-93b6-6d91cb5a0c9f)
<br>![39](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/9aa67bea-1968-4884-93a8-619f228eb82f)
<br>![40](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/237592e9-c431-4637-9115-c93d9733e495)
<br>![41](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/c08dd0a9-3255-4d4c-9112-05b9b88da68a)
<br>![42](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/b237c999-b179-41b7-aea4-769b5e087eb6)
<br>![43](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/95979705-fd72-45ad-8c57-83d8b0b90093)
<br>![44](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/dfccf438-7ee4-436c-b917-ee93c9a5dc52)
<br>![45](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/6a11ac0d-1baa-49c7-a756-e63667eb3ea4)
<br>![46](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/afde93b6-5abc-41d7-b766-fc0cb3fd9a49)
<br>![47](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/238cf589-e8ee-4afd-b962-e791e86c5ba8)
<br>![48](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/d387afa5-170a-4e16-b34d-c23197d57827)
<br>![49](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/c5952c84-af08-4d36-88c0-08a06e102d6d)
<br>![50](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/e94089c2-5399-4aed-b39f-8be61cbd914d)
<br>![51](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/d85659fb-a707-4b8c-8745-d2638d2217c2)
<br>![52](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/4cf01d46-b988-4288-bae2-d08902b307da)
<br>![53](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/ff4f1b6e-1e2c-4eab-9b62-3da4ebe566db)
<br>![54](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/ea85dbfa-fa53-4a2b-a8b5-6a48886421d8)
<br>![55](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/1588ae2d-7df2-4f22-ba6b-56c3db49bed7)

**DHCP Configuration**
<br>![56](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/f44bc771-297f-47d2-93f2-7acdd591ccb5)
<br>![57](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/34d8b67b-d9c0-4acc-af54-5fc8478c5e76)
<br>![58](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/14109148-c310-4c4f-8d28-026e41433946)
<br>![59](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/0ccb4ff4-e8f3-42b4-844c-0fdf6ecc0e34)
<br>![60](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/da5a5127-c183-4a38-a75e-903b5c4539cd)
<br>![61](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/0ccb2a35-e5b0-4bb3-ac94-cc2cf2a2e390)
<br>![62](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/3361fbb0-f98a-47b8-9bd1-a636ab3c805b)
<br>![63](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/ae895f47-034e-4d50-a680-c392a9edeb65)
<br>![64](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/31d835c0-2e47-45fb-97cd-11f786894ed0)
<br>![65](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/7263106c-15b4-4423-a89a-67317309c40c)
<br>![66](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/bc054525-fcc5-43d5-a7e4-5575bd7e7831)
<br>![67](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/385d47ea-fe67-4f3d-b960-c5964f8fe3ba)
<br>![68](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/21f7916f-3597-48be-b296-b111f87bff9c)
<br>![69](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/5050c198-25e2-44b8-bba2-63f9defd4882)
<br>![70](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/1c20684b-29b4-431e-94ba-2efd4ce44d87)
<br>![71](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/cedbcea7-6a7d-46ce-a786-3da251b58ae4)
<br>![72](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/e142ab75-9320-498f-bd76-4c741f913a74)
<br>![73](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/6326020e-401e-4cae-a5fc-839a8786787e)
<br>![74](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/227d00c0-5dbb-4a13-90ee-b87bd306dd6a)
<br>![75](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/12ec6126-e2fd-42f1-89d3-7ff96ee00511)
<br>![76](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/dd44ac91-dbc5-450e-ac85-2a6d1519e2b9)
<br>![77](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/9709ee9e-d426-4c70-b824-e6989865751f)
<br>![78](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/b8881808-09d9-4eec-8a18-8a43e14abe05)
<br>![79](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/09efc95b-b4b7-4305-aec8-8070d5eacfe6)
<br>![80](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/ff1ba62a-ea39-4ffa-be85-4c80ce66cf5a)

**IIS Configuration**
<br>![81](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/445ac488-7253-40e6-bc03-94c20e56b579)
<br>![82](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/a2a3709d-bb44-45c4-9888-030e3e6d2769)
<br>![83](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/8dac69b7-a978-478d-8ac2-c890cd1e0981)
<br>![84](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/d86880bd-8af9-4448-aa08-c81435c86358)
<br>![85](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/7f05e5a4-02e9-4b9a-8da2-043cec0f770e)
<br>![86](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/1872a271-719c-4976-a592-d7c735a8cc0e)
<br>![87](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/d60e7cbc-4694-4d72-a061-c481ab4a9da5)
<br>![88](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/584f269a-e5d4-4396-a0b3-bf850fd6ee14)
<br>![89](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/97de85d7-b354-4750-9a90-2a1f7f6a030b)
<br>![90](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/db0810e9-c7f7-4eeb-94a4-162cf1a0a6de)
<br>![91](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/a8fcd4aa-0816-41dd-b7a6-ddd49e56b210)
<br>![92](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/b11e557d-17b3-4bca-8aaa-a57423508090)
<br>![93](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/c748b7aa-6129-415f-9cc5-f352a53db467)
<br>![94](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/f311b567-2150-4bc2-aac5-84e97fdb695f)
<br>![95](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/ea1f2818-b33f-468c-9859-3cc0a44e2c89)
<br>![96](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/414becb8-3599-4aa2-87d7-ebcab3da4fd7)
<br>![97](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/534538b0-ffc8-41da-bc2d-d5562843ce9b)
<br>![98](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/f8bd307b-93c3-4973-928f-597700935112)
<br>![99](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/19ec8159-cd38-4d42-b0a3-1d2a329268a3)
<br>![100](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/5f8b98eb-56f8-4eb9-a54c-b78f694e92b2)
<br>![101](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/4b7961f9-a117-492e-a141-01a32e5dbdd7)
<br>![102](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/e10d0fa1-82e7-43bc-b868-e4118c3e49d9)
<br>![103](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/37e426a8-c818-4b7f-b98c-f8694bf6cf2f)
<br>![104](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/903d07d9-e500-47e6-9b19-fb6bff944ef4)

**FTP Configuration**
<br>![105](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/d3ebd8a6-9f85-4e84-8058-4ba966ba47c6)
<br>![106](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/236663df-8343-442b-b471-3e8b65d50dc4)
<br>![107](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/bf8f7e31-c2ba-45c3-b5d6-659c22c1af9c)
<br>![108](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/9e1949d1-1310-4692-bbeb-f7f422828690)
<br>![109](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/a68ed328-f373-4f4f-b911-6c24c689fcef)
<br>![110](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/1700ef6a-ba0f-4024-880c-3aa1c7612ffc)
<br>![111](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/43c41b2d-0e69-4a63-979c-3247c8851908)
<br>![112](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/08ce34f5-658a-4758-86b0-e1c8c14e99bb)
<br>![113](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/aef13116-226c-493d-ac89-cf39722cf146)
<br>![114](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/f421d8e4-5263-4b96-b1ee-450f32556f30)
<br>![115](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/4a091b32-0e06-4a30-b49d-6a1e9c1739c9)
<br>![116](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/44060197-ecf3-4910-9655-097134d2e7d9)
<br>![117](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/cdee8c10-c7a6-490d-9f7a-fc8bec71591b)
<br>![118](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/764d70b1-1ac3-44ee-bbfd-50e8093e8e30)
<br>![119](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/23b03cd4-0340-49c9-b297-af654cf551c3)
<br>![120](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/50785fa6-a4a9-4c82-bd17-12aa7aed21e0)
<br>![121](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/c8c22d75-4470-4e39-8723-59cce2be8e3f)
<br>![122](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/64da0a66-e781-474e-abc5-1ff858a307bc)
<br>![123](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/97e8748b-5bfb-4f71-8490-fdab9845b8c7)
<br>![124](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/fa22897c-bf31-4121-a5d9-81764ac31a8c)
<br>![125](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/f327ec12-82e6-44a7-803e-3016aa703ba4)
<br>![126](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/49dde0ce-d52f-4116-b4e1-4d8ecf1e1302)
<br>![127](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/8675e457-c886-43b4-bd06-16a2bdae6322)

**File Server Configuration**
<br>![128](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/633b15cb-7be0-4672-9058-896bcae0dc62)
<br>![129](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/acc5bd78-21ca-46a3-89b5-6ce0d83e3981)
<br>![130](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/3b2868f1-fa07-4788-8117-12c8cbd9cbcb)
<br>![131](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/99e6130e-b01b-4242-bcc4-95e6e0f71df1)
<br>![132](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/4a5c9bec-a9a0-48b2-a028-21cfd2dc7e6f)
<br>![133](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/323bbe17-7109-4fa5-8cb5-6c9ef47059f7)
<br>![134](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/f31813d9-add3-4a94-a76f-7aff20976e31)
<br>![135](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/30f09a18-80fd-4767-866e-468d12de9ec2)
<br>![136](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/d2cb46a3-acb8-4916-aef6-ec51a905005b)
<br>![137](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/1b93aac1-1b2a-46ab-853d-8670499ff9ec)
<br>![138](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/7925ab7e-189a-4d09-9940-55ffe8eb32e6)
<br>![139](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/f7b30a31-5f83-4579-b64f-a8e7ab56edc2)
<br>![140](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/afb37ce7-3047-45bb-9f78-43b08ffabc51)
<br>![141](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/f45cc98b-8386-4f55-836f-906cdc9949b2)
<br>![142](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/08ee1c01-d789-474b-a93b-f399ad013ff8)
<br>![143](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/8e19fa45-1b58-40fd-8e16-5388b2dcc6c7)
<br>![144](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/c8dd7f79-6d17-4f92-9e77-94a21f3e7f1e)
<br>![145](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/be893713-1498-41bf-aac9-11c6095a5eaf)

**DFS Configuration**
<br>![146](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/e5e1b477-a1e9-44ba-8afd-bb2f893f496e)
<br>![147](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/a481242c-d64c-4c62-bf27-ee1d8749f01b)
<br>![148](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/95ed0bef-8713-4fce-84d7-3891af7f3156)
<br>![149](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/2b3e3800-ce22-440d-bc19-d7765abcac06)
<br>![150](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/20912c36-9800-4884-9b65-06f556733ff2)
<br>![151](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/f8165b4b-4e5a-452d-8334-418726c803f8)
<br>![152](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/e366060a-0e27-457b-bae9-1ef36c41820e)
<br>![153](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/994fa7da-c178-420c-804e-b4895ef5f271)
<br>![154](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/3ef63169-69c2-4716-956a-fcea4d7f9720)
<br>![155](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/be931a07-8612-4602-9c49-6ce781091b5c)
<br>![156](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/405e91dc-1273-4d75-919e-2517db477ea1)
<br>![157](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/bcb81748-6d66-4607-951e-4b2be564b0ca)

**Failover Cluster Configuration**
<br>![158](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/29fe01ed-27ba-461a-a031-31e49ff95742)
<br>![159](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/7a2afaf3-5e81-44ca-88fd-6e0524dba27c)
<br>![160](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/1afd3322-ed7a-422e-8fd4-15758e23d92c)
<br>![161](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/f65a7734-cbb3-41df-b0e3-f78394bfd890)
<br>![162](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/6d06f427-d00e-48f6-bdc0-91ee202aa3dc)
<br>![163](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/85d4a548-036c-46f6-ae06-ba2761b19bc9)
<br>![164](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/e8cb6f81-84ce-4d25-a49e-33c8f7ede734)
<br>![165](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/ba323130-1611-4405-921e-27ea0504354b)
<br>![166](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/55d29303-5d45-4398-852e-5dba027bf5aa)
<br>![167](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/963ac51e-c0fb-4b3e-885e-a9b9a4f286dc)
<br>![168](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/e47a1fd2-a8d4-4224-8925-f3f343cc9a03)
<br>![169](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/85f24194-556b-4aa5-b051-0da770b8e374)
<br>![170](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/2525b688-451b-4d0d-8917-2414bc75e557)
<br>![171](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/1e82b963-cb2b-4772-a611-c9870cd6173b)
<br>![172](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/cdefb137-1e59-4db2-9402-284dbb83f1c7)
<br>![173](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/379beb1a-7b2b-4143-838a-73293e1c1b7a)
<br>![174](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/02b46e6d-0c18-4d17-a44a-4e79c096dd06)
<br>![175](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/b08c93ad-b87a-4609-b902-42a9e7d13829)
<br>![176](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/198ec50c-59cd-494e-8db3-efad17e68f94)
<br>![177](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/c9a01477-57b6-4cf4-bf92-f48e14330cba)
<br>![178](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/4ca9aa30-199b-4241-868d-387be2c2e1c9)
<br>![179](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/2736b661-f228-43af-9910-3c883c219a4d)
<br>![180](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/7318da17-0c99-4a16-b05e-6f893213ce80)
<br>![181](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/ac3440c5-cca3-415d-832e-eb1dc4f490b8)
<br>![182](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/73fd5288-11ef-4d4e-a22e-e09f418c03e7)
<br>![183](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/1051ac00-ace8-4274-930f-da803acec727)
<br>![184](https://github.com/jose-ambrosioo/system_administration_using_windows_server/assets/59221796/0434f5c5-ca7f-48f1-b6db-57dfdbf3e5bc)
