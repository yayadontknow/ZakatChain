# **ZakatChain Documentation**

# Figma Prototype: https://www.figma.com/proto/OsPTsVhqHyUo1Ubggc55cK/ZakatChain?node-id=0-1&t=vBWnpHgZtbfsuEwD-1

# Pitch Deck: https://docs.google.com/presentation/d/1SNhhHe7Y0sAAuDWM1ylQ1_sog4aG1jtA/edit?usp=sharing&ouid=101697955047506946782&rtpof=true&sd=true

## **Overview**

**ZakatChain** is a decentralized platform that utilizes blockchain technology to ensure transparency, trust, and accountability in the distribution of zakat (charitable donations) within the Muslim community. By leveraging **Solana Blockchain** for transaction transparency and **IPFS** (InterPlanetary File System) for data storage, ZakatChain allows donors, organizations, and vendors to track and verify every step of the zakat process — from donation to fulfillment.

---

## **Features**

1. **Transparent Zakat Distribution**  
   - Donors can track where their zakat goes, from the donation to the delivery of aid.
   - Organizations and vendors are verified through blockchain attestations.
   
2. **Verification Process**  
   - Organizations (e.g., orphanages, schools) and vendors (e.g., bookshops, suppliers) must submit their applications to the Majlis Agama (Religious Council) for approval.
   - Once approved, a **digital certificate** is issued and stored on **IPFS** for transparent verification.
   - The verification attestation is stored on the **Solana blockchain**, ensuring data integrity.

3. **Donation Tracking**  
   - Donors can see open zakat requests, such as a school asking for 100 books or an orphanage requesting 100 pencils.
   - Each donation is tracked on the Solana blockchain, allowing for real-time monitoring and updates.

4. **Fulfillment Confirmation**  
   - Once an organization receives the requested items (e.g., books, pencils), the fulfillment is confirmed and attested on the blockchain.
   - Donors are notified when their donation has been successfully delivered.

5. **Real-Time Impact Stats**  
   - ZakatChain provides real-time updates on the impact of donations. Donors can see how many people were helped, view live charts, and receive notifications about their contributions.

6. **IPFS and Blockchain Integration**  
   - IPFS is used to store the verification documents and fulfillment receipts, while the blockchain records the relevant metadata, such as timestamps, categories, and expiration dates.

---

## **System Architecture**

### **1. Entity Verification**

**Organizations and Vendors:**
- Organizations (e.g., schools, orphanages) and vendors (e.g., bookshops, suppliers) submit their application forms to the Majlis Agama for verification.
- Upon approval, a digital certificate is issued and stored on **IPFS**.
- The verification attestation is recorded on the **Solana blockchain** with details like category, timestamp, and expiration date.

### **2. Aid Request Submission**

**Organizations Request Aid:**
- Organizations create a request for aid (e.g., 100 books from Vendor A).
- The request is attested on the **Solana blockchain**, linking it to the requesting organization and vendor.
- The request includes details such as:
  - **Requester Wallet Address**  
  - **Vendor Wallet Address**  
  - **RequestID**  
  - **Items Requested**  
  - **Count**  

### **3. Donation Flow**

**Donors Contribute:**
- Donors browse the platform and choose to contribute to an open zakat request (e.g., "100 pencils for Orphanage X").
- Donations are made via cryptocurrency on the **Solana blockchain**.
- The smart contract tracks the total amount donated and links the donation to a specific request.

### **4. Vendor Fulfillment**

**Vendor Ships the Items:**
- Once a request is fully funded, the vendor (e.g., bookshop) delivers the items to the organization.
- The organization confirms the receipt of the items and attests the fulfillment on the blockchain.
- The confirmation includes:
  - **Requester Wallet Address**  
  - **Vendor Wallet Address**  
  - **RequestID**  
  - **Receipt IPFS hash**

### **5. Notification & Real-Time Updates**

**Donor Notifications:**
- When fulfillment is confirmed, donors are notified about the successful delivery of their contribution.
- Impact statistics and charts on the platform update in real-time to reflect the donation’s effect (e.g., “100 pencils delivered to Orphanage X”).