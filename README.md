# wp-config.php
<?php
/**
 * The base configuration for WordPress
 *
 * The wp-config.php creation script uses this file during the
 * installation. You don't have to use the web site, you can
 * copy this file to "wp-config.php" and fill in the values.
 *
 * This file contains the following configurations:
 *
 * * MySQL settings
 * * Secret keys
 * * Database table prefix
 * * ABSPATH
 *
 * @link https://codex.wordpress.org/Editing_wp-config.php
 *
 * @package WordPress
 */

// ** MySQL settings - You can get this info from your web host ** //
/** The name of the database for WordPress */
define('DB_NAME', 'wordpress');

/** MySQL database username */
define('DB_USER', 'fullsail');

/** MySQL database password */
define('DB_PASSWORD', 'Fullsail1');

/** MySQL hostname */
define('DB_HOST', 'localhost');

/** Database Charset to use in creating database tables. */
define('DB_CHARSET', 'utf8mb4');

/** The Database Collate type. Don't change this if in doubt. */
define('DB_COLLATE', '');

/**#@+
 * Authentication Unique Keys and Salts.
 *
 * Change these to different unique phrases!
 * You can generate these using the {@link https://api.wordpress.org/secret-key/1.1/salt/ WordPress.org secret-key service}
 * You can change these at any point in time to invalidate all existing cookies. This will force all users to have to log in again.
 *
 * @since 2.6.0
 */
define('AUTH_KEY',         'CR{/}C_W{L}jVleux.RL%>f!<tAZRTH< ejO?163w=>S0&c[3#YOAi*Je>;.V,#;');
define('SECURE_AUTH_KEY',  'E/(%IQiJkE&e/bz9r2s&F?tf5sp.)]Uk=4%PKx.H*5NtONCLLz$:q^g+*7M/hj-5');
define('LOGGED_IN_KEY',    'c.3Vjiv^_<JTLAmx;=33-c{6lCZ,BlMdWN&k]Cl/|*[qdzd)E/ZfyC6bI/]g9;=a');
define('NONCE_KEY',        'T(DLi]p:0TjBs_rcY9mF*X!H4-0/VB->=eVMyN#t#gjfayZcx4yc]*eAk[_TUJCP');
define('AUTH_SALT',        '-HJ48)A*hY!,00 RA!=C.(($;)Pm9AVuU%_n&yY8{KzF4A42NUZTIG__Sf:tQc~f');
define('SECURE_AUTH_SALT', 'Ars)+kHA+lFawzmnHlxe]]3z5;@VNwiL#P`?jFM-&=s#H3/}(}yZk6m[c?=@zt=}');
define('LOGGED_IN_SALT',   'lckCBJusG6}Ug@<MsePGD ,:gQKB~!8FJ&6N]~HZs>b(plx!1<7=g;:,=e& [Z*Z');
define('NONCE_SALT',       'm,0[%se+a`LdokChebfEf(+ys;j-&SGW}&&|AgIR#>ii>cL0Qn.<>sWo-tfiXg93');

/**#@-*/

/**
 * WordPress Database Table prefix.
 *
 * You can have multiple installations in one database if you give each
 * a unique prefix. Only numbers, letters, and underscores please!
 */
$table_prefix  = 'wp_';

/**
 * For developers: WordPress debugging mode.
 *
 * Change this to true to enable the display of notices during development.
 * It is strongly recommended that plugin and theme developers use WP_DEBUG
 * in their development environments.
 *
 * For information on other constants that can be used for debugging,
 * visit the Codex.
 *
 * @link https://codex.wordpress.org/Debugging_in_WordPress
 */
define('WP_DEBUG', false);

/* That's all, stop editing! Happy blogging. */

/** Absolute path to the WordPress directory. */
if ( !defined('ABSPATH') )
	define('ABSPATH', dirname(__FILE__) . '/');

/** Sets up WordPress vars and included files. */
require_once(ABSPATH . 'wp-settings.php');
