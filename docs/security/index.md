# Security

This section covers essential security configuration steps, including changing the default admin user credentials and setting up email authentication.

## Default Admin User

EPMware comes with a default admin user account that must be secured immediately after installation. This is a critical security step that should not be delayed.

!!! warning "Security Alert"
    The default admin account uses a well-known password. Change it immediately to prevent unauthorized access to your EPMware system.

## Change Password

Follow these steps to update the default admin user credentials:

### Access User Management

1. Navigate to **Security** → **Users**
2. Locate the **Admin** user in the user list
3. Right-click on the Admin user row
4. Select **Edit User** from the context menu

### Update Credentials

In the Edit User dialog:

1. **Change Password**
   - Enter a new strong password
   - Confirm the new password
   - Follow password complexity requirements

2. **Update Email Address**
   - Replace default email with administrator's email
   - This email receives system notifications

### Password Requirements

Your new password should meet these criteria:

| Requirement | Description |
|-------------|-------------|
| **Length** | Minimum 8 characters |
| **Uppercase** | At least one uppercase letter |
| **Lowercase** | At least one lowercase letter |
| **Numbers** | At least one numeric digit |
| **Special Characters** | At least one special character (!@#$%^&*) |
| **Uniqueness** | Cannot match previous 5 passwords |

!!! tip "Password Best Practices"
    - Use a password manager to generate and store strong passwords
    - Avoid using personal information
    - Don't reuse passwords from other systems
    - Change passwords regularly (every 90 days recommended)


## Next Steps

After securing the admin account:

1. Configure [Global Settings](../global-settings/) including email settings
2. Create additional user accounts
3. Set up roles and permissions
4. Enable audit logging

---

## Related Topics

- [Global Settings](../global-settings/)
- [User Management](../reference/)
- [Audit Logging](../reference/#audit-logging)
- [Password Policy](../reference/#password-policy)
