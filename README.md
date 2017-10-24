# states-india
States Name of India

# To fill dropdown using PHP
$states = json_decode(file_get_contents('states-india-master/states-of-india-v2.json')); 
													
foreach($states->states as $states){
    echo '<option value="' . $states->ISO . '">' . $states->name . '</option>';
}
