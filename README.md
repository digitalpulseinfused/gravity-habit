gravity-habit
=============

Gravity Form Submission To Infusionsoft 

<?php>
require_once("$isdk.php");

$app = newiSdk;

if ($app ->confg('ConnectionName')){


$difclientemail = $_GET ['difclientemail'] //CustomField
$reportnameholder = $_GET ['reportnameholder'] //CustomField
$referrer = $_GET ['referrer'] //CustomField
$source = $_GET ['source'] //CustomField
$timeframe = $_GET ['timeframe'] //CustomField
$agentoffice = $_GET ['agentoffice'] //CustomField
$agentphone = $_GET ['agentphone'] //CustomField
$agentemail = $_GET ['agentemail'] //CustomField
$agentlname = $_GET ['agentlname'] //CustomField
$agentfname = $_GET ['agentfname'] //CustomField
$otherinfo = $_GET ['otherinfo'] //CustomField
$extbldg = $_GET ['extbldg'] //CustomField
$hsesize = $_GET ['hsesize'] //CustomField
$trust = $_GET ['trust'] //CustomField
$mobphone = $_GET ['mobphone'] 
$workph = $_GET ['workph']
$confirmwithclient = $_GET ['confirmwithclient'] //Tag
$howsold = $_GET ['howsold'] //CustomField
$bthm = $_GET ['bthm'] //CustomField
$storey = $_GET ['storey'] //CustomField
$city = $_GET ['city'] 
$suburb = $_GET ['suburb'] 
$street = $_GET ['street']
$sitecity = $_GET ['sitecity']
$sitesuburb = $_GET ['sitesuburb']
$sitestreet = $_GET ['sitestreet']
$email = $_GET ['email']
$Lname = $_GET ['Lname']
$Fname = $_GET ['Fname']


$update = array('difclientemail' => $difclientemail, '_NameHolderOfInspection ' => $reportnameholder, 
				'_OtherSource ' => $referrer, 'Source' => $source, '_Timeframe' => $timeframe,
			    '_AgentOffice' => $agentoffice, '_AgentPhone' => $agentphone, '_AgentEmail' => $agentemail,
			    '_AgentLastName' => $agentlname, '_AgentFirstName' => $agentfname, '_Notes' =>$otherinfo,
			    '_ExternalBuildings' => $extbldg, '_HouseSize' => $hsesize, '_EstateTrustName0' => $trust, 'Phone2' => $mobphone,
			    'Phone2' => $workph, 'Confirmwithclient' => $confirmwithclient, 'Howsold' => $howsold,
			    'Bthm' = > $bthm, 'Storey' = >$storey, 'City' => $city, 'Street' => $street, 'Sitecity' => $sitecity,
			    'Sitesuburb' => $sitesuburb, 'Sitestreet' => $sitestreet, 'Email' => $email, 'Lname' => $Lname, 'Fname' => $Fname);
			    )


$app->addWithDupCheck($update, 'Email');





if ($






// Add tags -  376 = Filled Out By 3rd Party
// 374 = Agreed To T & C's

//Sample code below
$contactId = 406;
$groupId = array("456", "376");

$result = $app->grpAssign($contactId, $groupId);

header('Location: http://thehabit.co.nz/th...');

} else

echo "You are connected";

}
