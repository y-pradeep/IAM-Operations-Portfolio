# Configure SAML-Based SSO

## Objective

To configure Security Assertion Markup Language (SAML) based Single Sign-On (SSO) between Microsoft Entra ID and an enterprise application, enabling users to authenticate using their Microsoft Entra ID credentials and securely access the application without managing separate usernames and passwords.

---

## Business Requirement

Organizations require centralized authentication for business applications to improve security, simplify user access, and reduce administrative overhead. SAML-based SSO enables federated authentication by allowing Microsoft Entra ID to act as the Identity Provider (IdP) while the application functions as the Service Provider (SP).

Implementing SAML SSO helps organizations:

- Provide seamless user access to enterprise applications.
- Centralize authentication and identity management.
- Improve security through controlled access policies.
- Reduce password-related support requests.
- Enforce Microsoft Entra ID security controls such as Conditional Access and Multi-Factor Authentication.
- Simplify user lifecycle management and deprovisioning.

---

## Steps of the Task

### Step 1: Sign in to Microsoft Entra Admin Center

1. Open a web browser.
2. Navigate to **https://entra.microsoft.com**.
3. Sign in using an account assigned one of the following roles:
   - Global Administrator
   - Cloud Application Administrator
   - Application Administrator
<img width="1917" height="961" alt="MS Entra Admin Center" src="https://github.com/user-attachments/assets/523031bc-6df8-4280-928f-33360f168b21" />

---

### Step 2: Create or Select an Enterprise Application

1. Navigate to **Identity** > **Applications** > **Enterprise Applications**.
2. Click **+ New Application**.
3. Search for the required application from the Microsoft Entra application gallery.

   **OR**

4. Select **Create your own application** for a custom SAML application.
5. Enter the application name.
6. Click **Create**.

<img width="1913" height="954" alt="image" src="https://github.com/user-attachments/assets/9104529a-e546-4a68-9ae0-156d05754079" />

---

### Step 3: Configure Single Sign-On

1. Open the Enterprise Application.
2. Select **Single Sign-On**.
3. Choose **SAML** as the SSO method.

<img width="1911" height="938" alt="image" src="https://github.com/user-attachments/assets/a98f2bba-7d75-44a9-bd8f-e95af719a1d8" />

---

### Step 4: Configure Basic SAML Settings

1. Under **Basic SAML Configuration**, click **Edit**.
2. Enter the application-specific values provided by the vendor.

| Setting | Description |
|----------|-------------|
| Identifier (Entity ID) | Unique identifier of the application | 
| Reply URL (Assertion Consumer Service URL) | URL that receives SAML responses | 
| Sign-On URL | Application login URL (Optional) | (ex: https://samltestapp.azurewebsites.net/)
| Relay State | Optional application state information |
| Logout URL | Application logout endpoint |

Entity ID : (ex: https://samltestapp.azurewebsites.net)
Assertion Consumer Service URL: (ex: https://samltestapp.azurewebsites.net/SAML/Consume)

<img width="1917" height="959" alt="image" src="https://github.com/user-attachments/assets/1245277e-427d-4d7c-99bf-6944ca72839a" />

3. Click **Save**.

---

### Step 5: Configure User Attributes and Claims

1. Navigate to **Attributes & Claims**.
2. Review the default claims.
3. Add or modify claims as required by the application.
4. Configure additional attributes if requested by the application vendor.

<img width="1917" height="952" alt="image" src="https://github.com/user-attachments/assets/893c1eab-4ba7-47d8-bde2-3da28f85df85" />

#### Common SAML Claims

```text
user.userprincipalname
user.mail
user.givenname
user.surname
user.displayname
```

5. Save the configuration.

---

### Step 6: Download SAML Metadata and Certificate

1. Navigate to the **SAML Certificates** section.
2. Download the required documents:

   - Certificate (Base64)
   - Federation Metadata XML

3. Record the following URLs:

   - Login URL
   - Microsoft Entra Identifier
   - Logout URL

4. Share the required information with the application administrator.
   
<img width="1912" height="233" alt="image" src="https://github.com/user-attachments/assets/15ba3491-156f-424b-aad8-1bfad5206466" />

---

### Step 7: Configure the Service Provider Application (If Required)

1. Log in to the target application administration portal.
2. Navigate to SAML Authentication settings.
3. Provide the Microsoft Entra ID details:

| Parameter | Source |
|------------|---------|
| Entity ID | Microsoft Entra ID |
| Login URL | Microsoft Entra ID |
| Logout URL | Microsoft Entra ID |
| Signing Certificate | Downloaded Certificate |
| Metadata XML | Downloaded Metadata File |

4. Save the configuration.

> Note: This step is required only for production applications such as Salesforce, ServiceNow, SAP, Workday, AWS, and other third-party applications.
>
> It is not required when using SAML test applications for lab or learning purposes.
---

### Step 8: Assign Users and Groups

1. Return to the Enterprise Application in Microsoft Entra ID.
2. Select **Users and Groups**.
3. Click **+ Add User/Group**.
4. Select the required users or groups.
5. Click **Assign**.

<img width="1917" height="947" alt="image" src="https://github.com/user-attachments/assets/ebdcc738-e4ea-4fd2-9705-7ab60842b1b6" />


---

### Step 9: Test SAML Single Sign-On

1. Navigate to **Single Sign-On**.
2. Select **Test**.

   <img width="1917" height="941" alt="image" src="https://github.com/user-attachments/assets/cc0071ec-af13-4870-ae93-4ddc4a530045" />

4. Launch the application from My Apps Portal or the Enterprise Application page.
5. Verify successful authentication.
6. Confirm the user is redirected to the application without credential prompts.

<img width="1902" height="1019" alt="image" src="https://github.com/user-attachments/assets/bbc4edcb-0ab5-4bfb-8da3-c3555ca267dc" />

---

### Step 10: Validate Application Access

Verify the following:

- Users can successfully access the application.
- Authentication occurs through Microsoft Entra ID.
- Required claims are passed correctly.
- Assigned users and groups can access the application.
- Unassigned users are denied access.
- Conditional Access and MFA policies are enforced if configured.

---

---

## Expected Outcome

A SAML-based Single Sign-On integration is successfully configured between Microsoft Entra ID and the target application. Users can securely authenticate using their Microsoft Entra ID credentials and access the application without managing separate login credentials, while administrators maintain centralized access control and security governance.
