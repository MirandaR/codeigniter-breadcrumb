# CodeIgniter-Breadcrumb

CodeIgniter-Breadcrumb is a library that helps your build HTML breadcrumbs with CodeIgniter.

This version is customised to work with breadcrumbs using Twitter Bootstrap.


## Requirements

* CodeIgniter 2.0.x


## Example

	// load library
	$this->load->library('breadcrumb');
	
	// add breadcrumbs
	$this->breadcrumb->append('Page', 'page');
	
	// prepend breadcrumbs
	// link parameter is optional
	$this->breadcrumb->prepend('Home');
	
	// populate multiple
	$this->breadcrumb->populate(array(
		'Admin' => 'admin',
		'Members' => 'admin/members',
		'All'
	));
	
	// put this line in view to output
	$this->breadcrumb->output();
