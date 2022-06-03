<?php

abstract class Item
{
	protected $id;
	protected $metalType;
	protected $lethality;
	protected $noOfHandsNeeded;
    
	public function getId()
	{
    	return $this->id;
	}
    
	public function getMetalType()
	{
    	return $this->metalType;
	}
    
	public function getLethality()
	{
    	return $this->lethality;
	}

    public function setLethality($lethality)
    {
        $this->lethality = $lethality;
    }
    
	public function getNoOfHandsNeeded()
	{
    	return $this->noOfHandsNeeded;
	}
    
	public function setMetalType($metal)
	{
    	$this->metalType = $metal;
	}
}

class Sword extends Item
{
	public function __construct()
	{
    	$this->id = 1;
    	$this->metalType = "bronze";
    	$this->lethality = "big";
    	$this->noOfHandsNeeded = 1;
	}
}

class TwoHandAxe extends Item
{
	public function __construct()
	{
    	$this->id = 2;
    	$this->metalType = "steel/wood";
    	$this->lethality = "bigest";
    	$this->noOfHandsNeeded = 2;
	}
}

function test()
{
	$sword = new Sword();
	$axe = new TwoHandAxe();
    
	$clonedAxe = clone $axe;
    $clonedSword = clone $sword;
    $clonedSword->setLethality("Deadly");
	$clonedAxe->setMetalType("Iron/wood");
	echo $clonedAxe->getMetalType();
	echo $clonedSword->getLethality();
	
}

test();

?>
