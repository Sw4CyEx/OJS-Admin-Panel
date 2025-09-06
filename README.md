# OJS Admin Panel

A modern, elegant admin panel for Open Journal Systems (OJS) user management with a sleek dark theme and animated interface.

![OJS Admin Panel](https://cdn.save.moe/b/mS1x0Z3r.png)
![OJS Admin Panel](https://cdn.save.moe/b/IyIGm2R1.png)

## 🚀 Features

- **User Management**: Create, view, edit, and delete users with Administrator and Manager roles
- **Role Counters**: Real-time counters showing the number of administrators and managers
- **Password Management**: Secure password editing for all users through modal interface
- **Modern UI**: Elegant black and blue theme with animated elements and particle effects
- **OJS Compatibility**: Works with OJS 2.4-3.x database structures
- **Responsive Design**: Optimized for desktop and mobile devices
- **Single File**: Complete functionality in one PHP file for easy deployment

## 🎨 Design Features

- Animated gradient backgrounds and glowing text effects
- Floating particle animations for modern aesthetics
- Smooth hover effects and transitions
- Glass-morphism UI elements with backdrop blur
- Dynamic loading animations
- Professional dark theme with blue accents

## 📋 Requirements

- PHP 7.4 or higher
- MySQL/MariaDB database
- OJS 2.4-3.x installation
- Web server (Apache/Nginx)

## 🛠️ Installation

1. **Download the file**
   ```bash
   wget https://github.com/Sw4CyEx/OJS-Admin-Panel/raw/main/ojs_admin_panel.php
   ```

2. **Upload to your web server**
   - Place `ojs_admin_panel.php` in your web directory
   - Ensure PHP has read/write permissions

3. **Configure database connection**
   - Open `ojs_admin_panel.php` in a text editor
   - Update the database configuration at the top of the file:
   ```php
   $db_host = 'localhost';        // Your database host
   $db_name = 'your_ojs_database'; // Your OJS database name
   $db_user = 'your_username';     // Your database username
   $db_pass = 'your_password';     // Your database password
   ```

4. **Access the panel**
   - Navigate to `http://yourdomain.com/ojs_admin_panel.php`
   - Start managing your OJS users!

## 🔧 Configuration

### Database Settings
Update these variables at the top of the PHP file:

```php
// Database Configuration
$db_host = 'localhost';
$db_name = 'your_ojs_database';
$db_user = 'your_username';
$db_pass = 'your_password';
```

### OJS Version Compatibility
The panel automatically detects your OJS version and uses the appropriate database schema:
- **OJS 3.x**: Uses `user_groups` and `user_user_groups` tables
- **OJS 2.x**: Uses `roles` table structure

## 📖 Usage

### Creating Users
1. Fill in the "Create New User" form
2. Select the appropriate role (Administrator/Manager)
3. Click "Create User"
4. The user will be created with proper OJS permissions

### Managing Existing Users
- **View Users**: All users with Administrator/Manager roles are displayed in the table
- **Change Password**: Click the "Change Password" button to update user passwords
- **Delete Users**: Click the "Delete" button to remove users from the system

### Role Counters
The dashboard displays real-time counters for:
- Total Administrators
- Total Managers

## 🗄️ Database Compatibility

### Supported OJS Versions
- ✅ OJS 2.4.x
- ✅ OJS 3.0.x
- ✅ OJS 3.1.x
- ✅ OJS 3.2.x
- ✅ OJS 3.3.x
- ✅ OJS 3.4.x

### Database Tables Used
**OJS 3.x:**
- `users` - User account information
- `user_groups` - Role definitions
- `user_user_groups` - User role assignments

**OJS 2.x:**
- `users` - User account information
- `roles` - User role assignments

## 🔒 Security Features

- **Password Hashing**: Uses PHP's secure password hashing
- **SQL Injection Protection**: Prepared statements for all database queries
- **Input Validation**: Server-side validation for all user inputs
- **Error Handling**: Comprehensive error handling with user-friendly messages

## 🐛 Troubleshooting

### Common Issues

**Database Connection Error**
```
SQLSTATE[HY000] [1045] Access denied
```
- Check database credentials in the configuration section
- Ensure database user has proper permissions

**Table Not Found Error**
```
SQLSTATE[42S02]: Base table or view not found
```
- Verify OJS database name is correct
- Check that OJS is properly installed

**Context ID Constraint Error**
```
Column 'context_id' cannot be null
```
- This has been fixed in the latest version
- Ensure you're using the updated code

### Debug Mode
To enable debug mode, add this line after the database configuration:
```php
$debug_mode = true;
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b Sw4CyEx/OJS-Admin-Panel`)
3. Commit your changes (`git commit -m 'Add Sw4CyEx/OJS-Admin-Panel'`)
4. Push to the branch (`git push origin Sw4CyEx/OJS-Admin-Panel`)
5. Open a Pull Request

## 📝 Changelog

### v1.0.0
- Initial release with full OJS compatibility
- Modern dark theme with animations
- Support for OJS 2.4-3.x versions
- User creation, editing, and deletion
- Role-based user management

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Open Journal Systems (OJS) community
- PKP (Public Knowledge Project) for OJS development
- Contributors and testers

## 📞 Support

If you encounter any issues or have questions:
1. Check the troubleshooting section above
2. Open an issue on GitHub
3. Provide detailed error messages and your OJS version

---

**Made with ❤️ for the OJS community**
