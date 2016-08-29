# Random-Story-Project
/*This project takes you through an exciting story filled with Pokemon, zombies, and weird logic! 
 *Time to go on an adventure!
 *Improvements to Consider: make code easier to navigate, create constants instead of magic numbers, come up with 
 *random outcomes
 */
package story.project;

/**
 *
 * @author bigmak712
 */

/* NOTE: This project was created during the summer before I went off to college so please excuse the extreme lack
 * of commenting (I didn't know any better!!!) and the very confusing format. I just wanted to do see what I could do 
 * with the knowledge that I gained from my high school computer science class.
 */

import java.util.Scanner;
public class StoryProject {

    public static void main(String[] args) {
    
        Scanner reader = new Scanner(System.in);
        String menu, menu1, menu2, menu3, menu4, menu5, menu6, menu7, menu8, menu9, menu10, menu11, menu12, menu13;
        String menuOption;
        
        //beginning of the story
        
        System.out.println("One day, you wake up in a forest with nothing but your clothes, a Masterball, and                                   $1000." + "\nWhat do you choose to do?");
        
        menu = "1. Stay in the forest and chill out."
             + "\n2. Go out and try to find random Pokemon."
             + "\n3. Escape the forest in the hopes of finding civilization.";
        menu1 = "1. Go out and challenge the Elite Four with your mighty Magikarp."
              + "\n2. Train your Magikarp until it evolves into a Gyarados."
              + "\n3. Cut it up and sell the Magikarp pieces as sushi.";
        menu2 = "1. Jump out the window because you're bored."
              + "\n2. Go out and try to find some random Pokemon."
              + "\n3. Stay in your hotel room and chill out.";
        menu3 = "1. Go catch another Magikarp."
              + "\n2. Cut up the dead Magikarp and sell the pieces as \"fresh\" sushi." 
              + "\n3. Go back into the forest to look for more masterballs.";
        menu4 = "1. Go over to Costco and try to live off of all of the food in the hopes that the zombies don't attack you."
              + "\n2. Go over to Sam's Club and try to live off of all of the food in the hopes that the zombies                          don't attack you."
              + "\n3. Give up and just get bitten so that you don't have to worry about being chased by zombies.";
        menu5 = "1. Try and climb onto the roof and hope the zombies don't follow you."
              + "\n2. Try and pay off the zombies so that they don't eat you."
              + "\n3. Start eating the zombies and show them WHO EATS WHO!!!";
        menu6 = "1. Go over to Costco and hang out with the people over there."
              + "\n2. Go out and try to find some weapons."
              + "\n3. Fly over to China in search for a zombie cure.";
        menu7 = "1. Charge into the crowd of zombies going rapid fire with your Nerf gun."
              + "\n2. Try and barricade yourself inside Toys-R-Us."
              + "\n3. Imitate the zombies and hope that you blend in.";
        menu8 = "1. Go to Costco to get more food."
              + "\n2. Go to China to find a zombie vaccine."
              + "\n3. Take another nap in the \"My Little Pony\" section of Toys-R-Us.";
        menu9 = "1. Go eat some Chinese dim-sum."
              + "\n2. Consult a Buddhist monk on how to cure the zombies."
              + "\n3. Find a dead Magikarp and chop it into pieces to sell as sushi.";
        menu10 = "1. Invite the zombies to eat with you."
               + "\n2. Rub their bellies for good luck."
               + "\n3. Start eating the zombies and show them WHO EATS WHO!!!";
        menu11 = "1. Go out and try to cure the zombies by rubbing their bellies."
               + "\n2. Go eat some Chinese dim-sum."
               + "\n3. Decide to stay at the Buddhist monestary to become a monk.";
        menu12 = "1. Invite the zombies to become Buddhist monks."
               + "\n2. Start rubbing their bellies for good luck."
               + "\n3. Challenge them to a dance battle.";
        menu13 = "1. Travel around the world and distribute the cure."
               + "\n2. Try some of the Pikachu stew."
               + "\n3. Start dancing to celebrate.";
        menuOption="5";
        System.out.println(menu);
        menuOption=reader.nextLine();
        System.out.println();
        outerloop:
        while(menuOption!="-1"){
            if(menuOption.equals("1")){
                System.out.println("You go over to a pond and start playing peek-a-boo with yourself. Then you start climbing up trees because you think you're Spiderman. \nThen you go to sleep for a couple of hours. After you wake up, you become bored. \nWhat do you choose to do?");
                System.out.println(menu);
                menuOption=reader.nextLine();
                System.out.println();
            }
            else if(menuOption.equals("2")){
                menuOption="5";
                System.out.println("After searching for many miles, you discover a strange cave filled with Pokemon. As you explore the cave, you find many legendary Pokemon \nsuch as Mew, Mewtwo and even..MewTHREE!!! However all of them pale in comparison to the rarest of them all - Magikarp. So after countless \nhours trying to fight against Magikarp's mighty Splash attack, you are finally able to capture it with your Masterball. \nWhat do you choose to do?");
                System.out.println(menu1);
                menuOption=reader.nextLine();
                System.out.println();
                innerloop:
                while(menuOption!="-1"){
                    if(menuOption.equals("1")){
                        menuOption="5";
                        System.out.println("Sadly, your Magikarp dies after being hit by a super effective Thunderbolt from a Lvl 100 Pikachu. RIP Magikarp... \nWhat do you choose to do?");
                        System.out.println(menu3);
                        menuOption=reader.nextLine();
                        System.out.println();
                        while(menuOption!="-1"){
                            if(menuOption.equals("1")){
                                System.out.println("Unfortunately, you do not have a Masterball to catch another all-powerful Magikarp. \nWhat do you choose to do?");
                                System.out.println(menu3);
                                menuOption=reader.nextLine();
                                System.out.println();
                            }
                            else if(menuOption.equals("2")){
                                menuOption="3";
                                break;
                            }
                            else if(menuOption.equals("3")){
                                System.out.println("You go back into the forest that you woke up in and find another Masterball guarded by a mystical being. You challenge it to a \nrock-paper-scissors battle and after two days of not being able to beat it, the mystical being pities you and decides to just \ngive you the Masterball. \nWhat do you choose to do?");
                                System.out.println(menu);
                                menuOption=reader.nextLine();
                                System.out.println();
                                break innerloop;
                            }
                            else{
                                System.out.print("Error. Enter one of the numbered options below.\n" + menu3);
                                menuOption=reader.nextLine();
                            }
                        }
                    }
                    else if(menuOption.equals("2")){
                        System.out.println("You go deep within the mountains to train and consult multiple Pokemon masters, but after leveling it up countless times, it refuses \nto evolve. \nWhat do you choose to do?");
                        System.out.println(menu1);
                        menuOption=reader.nextLine();
                        System.out.println();
                    }
                    else if(menuOption.equals("3")){
                        menuOption="5";
                        System.out.println("After selling all of the Magikarp sushi pieces to people, you realize that the sushi is causing people to turn into zombies. As a result,\nyou have started a zombie apocalypse. \nWhat do choose to do?");
                        System.out.println(menu4);
                        menuOption=reader.nextLine();
                        System.out.println();
                        while(menuOption!="-1"){
                            if(menuOption.equals("1")){
                                menuOption="5";
                                System.out.println("Going to Costco sounds like a great idea...but everyone else is thinking the exact same thing. So, when you get there, Costco is already \nsuper crowded. As you struggle to try to find some food, a whole bunch of zombies start overrunning Costco and they begin infecting \neveryone. \nWhat do you choose to do?");
                                System.out.println(menu5);
                                menuOption=reader.nextLine();
                                System.out.println();
                                while(menuOption!=("-1")){
                                    if(menuOption.equals("1")){
                                        System.out.println("As you start making your way to the roof, five zombies begin chasing you. You quickly grab a safety buddy to run with you. Just as the \nfive zombies are about to reach you, you sprint ahead leaving behing your horizontally-challenged safety buddy behind to get eaten by \nthe zombies. You finally make it up to the roof where you see the Terminator waiting for you in his chopper. One of the zombies pops up \nbehind you and the Terminator starts shooting at it. But then he misses and kills you by accident. \nTHE END");
                                        break outerloop;
                                    }
                                    else if(menuOption.equals("2")){
                                        System.out.println("You start making it rain and surprisingly are willing to accept the money as payment. You have now achieved the status of SWAGGYSWAG-I-\nGOT-MONEY-IN-THE-BAG Master. As you stroll out of Costco with style listening to those other poor souls getting bitten, you fall on \nyour face and die. \nTHE END");
                                        break outerloop;
                                    }
                                    else if(menuOption.equals("3")){
                                        System.out.println("Well, the zombies eat you. \nTHE END");
                                        break outerloop;
                                    }
                                    else{
                                        System.out.println("Error. Enter one of the numbered options below.\n" + menu5);
                                        menuOption=reader.nextLine();
                                        System.out.println();
                                    }
                                }
                            }
                            else if(menuOption.equals("2")){
                                menuOption="5";
                                System.out.println("You is smart. When you go to Sam's Club, you discover that no one is there because everyone went to Costco. So, you begin taking all of \nthe supplies there. \nWhat do you choose to do?");
                                System.out.println(menu6);
                                menuOption=reader.nextLine();
                                System.out.println();
                                midouterloop:
                                while(menuOption!="-1"){
                                    if(menuOption.equals("1")){
                                        break;
                                    }
                                    else if(menuOption.equals("2")){
                                        menuOption="5";
                                        System.out.println("You go over to Toys-R-Us in order to get an all-powerful Nerf gun. When you get there, you discover that no one is at Toys-R-Us. So, \nyou help yourself to the best Nerf guns you can find. As you exit the store, you see a crowd of zombies slowly approaching you. \nWhat do you choose to do?");
                                        System.out.println(menu7);
                                        menuOption=reader.nextLine();
                                        System.out.println();
                                        midinnerloop:
                                        while(menuOption!="-1"){
                                            if(menuOption.equals("1")){
                                                menuOption="5";
                                                System.out.println("As you charge into the hoard of zombies firing you Nerf gun, it turns out to be super effective! After a short two minutes, the whole \ngroup of zombies is dead on the ground. Feeling very tired, you eat a bunch of frozen Hot Pockets and Pizza Rolls that you got from \nSam's Club. \nWhat do you choose to do?");
                                                System.out.println(menu8);
                                                menuOption=reader.nextLine();
                                                System.out.println();
                                                while(menuOption!="-1"){
                                                    if(menuOption.equals("1")){
                                                        break midouterloop;
                                                    }
                                                    else if(menuOption.equals("2")){
                                                        menuOption="3";
                                                        break midinnerloop;
                                                    }
                                                    else if(menuOption.equals("3")){
                                                        System.out.println("You curl up right next to a rainbow pony toy and you cover yourself with pony-themed blankets. As night falls, more and more zombies \nstart to roam the streets. You think you are safe but what you didn't know is that these zombies are obsessed with \"My Little Pony\". \nWhen the zombies walk in to Toys-R-Us and see you hogging all of the \"My Little Pony\" toys, they get super angry and they eat you in \nyour sleep. \nTHE END");
                                                        break outerloop;
                                                    }
                                                    else{
                                                        System.out.println("Error. Enter one of the numbered options below\n" + menu8);
                                                        menuOption=reader.nextLine();
                                                        System.out.println();
                                                    }
                                                }
                                            }
                                            else if(menuOption.equals("2")){
                                                System.out.println("As you barricade the door with various toys, you hear other zombies coming in through the back door. Realizing that you are stuck, you \ntry hiding in the \"My Little Pony\" section. However, zombies love their little pony toys, so when they see you cuddling with all of \nthose cute, fluffy ponies, they all jump you and start eating you. \nTHE END");
                                                break outerloop;
                                            }
                                            else if(menuOption.equals("3")){
                                                System.out.println("You ain't no zombie, so the zombies eat you.\nTHE END");
                                                break outerloop;
                                            }
                                            else{
                                                System.out.println("Error. Enter one of the numbered options below\n" + menu7);
                                                menuOption=reader.nextLine();
                                                System.out.println();
                                            }
                                        }
                                    }
                                    else if(menuOption.equals("3")){
                                        menuOption="5";
                                        System.out.println("You escape the zombie-infested lands and fly over to China in your private jet. Onboard you learn that all of the countries in the world \nhave zombies except for China. When you arrive in China, you have many options on what you can do. \nWhat do you choose to do?");
                                        System.out.println(menu9);
                                        menuOption=reader.nextLine();
                                        System.out.println();
                                        while(menuOption!="-1"){
                                            if(menuOption.equals("1")){
                                                menuOption="5";
                                                System.out.println("You go out to the world's most famous Chicken restaurant: Panda Express. You order a large bowl of their original orange chicken and \ntheir special of the day: Pikachu stew. Right when you're about to start eating, you see some random guy outside selling Magikarp sushi. \nBefore you can say anything, you see people outside collapsing and turning into zombies. As a couple of them eat the people outside, \nsome   of the zombies head into the restaurant. \nWhat do you choose to do?");
                                                System.out.println(menu10);
                                                menuOption=reader.nextLine();
                                                System.out.println();
                                                while(menuOption!="-1"){
                                                    if(menuOption.equals("1")){
                                                        menuOption="5";
                                                        System.out.println("You invite the zombies to eat with you and they graciously accept. When they start eating the Pikachu stew, all of  the zombies start \nthrowing up because it's so bad. However, they all throw up the Magikarp sushi and as a result they turn back into regular humans. \nYou have found the cure! \nWhat do you choose to do?");
                                                        System.out.println(menu13);
                                                        menuOption=reader.nextLine();
                                                        System.out.println();
                                                        while(menuOption!="-1"){
                                                            if(menuOption.equals("1")){
                                                            System.out.println("You fly all around the world pouring buckets of Pikachu stew on random zombies from your private jet. As a result, all of the zombies \nstart throwing up and they turn back into regular human beings. \nCONGRATULATIONS!!! YOU BEAT THE GAME!!!");
                                                            break outerloop;
                                                            }
                                                            else if(menuOption.equals("2")){
                                                                System.out.println("As you start eating the Pikachu stew, you can feel you heart beating faster. Your body starts shaking and then you start throwing up all \nover the floor. You reach for water but then you actually grabbed the Pikachu stew and you start chugging it. You fall to the floor gasping \nfor air and then... you die. You should've known better than to eat Pikachu stew. \nTHE END");
                                                                break outerloop;
                                                            }
                                                            else if(menuOption.equals("3")){
                                                                System.out.println("You start doing a bunch of b-boy moves like the windmill and the coffee-grinder but then you slip on some of the zombie throw-up and \nfall on your face and die.  \nTHE END");
                                                                break outerloop;
                                                            }
                                                            else{
                                                                System.out.println("Error. Enter one of the numbered options below\n" + menu13);
                                                                menuOption=reader.nextLine();
                                                                System.out.println();
                                                            }
                                                        }
                                                    }
                                                    else if(menuOption.equals("2")){
                                                        System.out.println("You go up to one of the zombies and start rubbing their bellies while chanting in Chinese. The zombie starts shaking and then he begins \nto glow. You start rubbing faster because you think it's working but then... the zombie blows up and kills you. \nTHE END");
                                                        break outerloop;
                                                    }
                                                    else if(menuOption.equals("3")){
                                                        System.out.println("Well, the zombies eat you. \nTHE END");
                                                        break outerloop;
                                                    }
                                                    else{
                                                        System.out.println("Error. Enter one of the numbered options below\n" + menu10);
                                                        menuOption=reader.nextLine();
                                                        System.out.println();
                                                    }
                                                }
                                            }
                                            else if(menuOption.equals("2")){
                                                menuOption="5";
                                                System.out.println("You go to a Buddhist monestary deep within the mountains. There you find a wise monk meditating. You ask him about how to cure the \nzombies and he tells you to rub their bellies in order for the Buddha's good luck to drive out the bad zombie luck out of them which \nwould restore them back to being regular human beings. \nWhat do you choose to do?");
                                                System.out.println(menu11);
                                                menuOption=reader.nextLine();
                                                System.out.println();
                                                while(menuOption!="-1"){
                                                    if(menuOption.equals("1")){
                                                        System.out.println("You go up to one of the zombies and start rubbing their bellies while chanting in Chinese. The zombie starts shaking and then he begins \nto glow. You start rubbing faster because you think it's working but then... the zombie blows up and kills you. \nTHE END");
                                                        break outerloop;
                                                    }
                                                    else if(menuOption.equals("2")){
                                                        menuOption="1";
                                                        break;
                                                    }
                                                    else if(menuOption.equals("3")){
                                                        menuOption="5";
                                                        System.out.println("You committ yourself to learning the way of the Buddha. You shave your head and start wearing orange robes. One day, when you're reciting \nancient Chinese poems with the wise monk, zombies start climbing the mountains in order to get to you. \nWhat do you choose to do?");
                                                        System.out.println(menu12);
                                                        menuOption=reader.nextLine();
                                                        System.out.println();
                                                        while(menuOption!="-1"){
                                                            if(menuOption.equals("1")){
                                                                System.out.println("You invite the zombies to become monks, but they have too much zombie bad luck. They are repulsed by your bald head and orange robe so \nthey decide to leave you alone. As you escort them outside of the monestary, you trip on one of the steps and fall on your face and die. \nTHE END");
                                                                break outerloop;
                                                            }
                                                            else if(menuOption.equals("2")){
                                                                System.out.println("You go up to one of the zombies and star rubbing their bellies while chanting in Chinese. The zombies starts shaking and then he begins \nto glow. You start rubbing faster because you think it's working but then... the zombie blows you up and kills you. \nTHE END");
                                                                break outerloop;
                                                            }
                                                            else if(menuOption.equals("3")){
                                                                System.out.println("You challenge one of the zombies and start b-boying with the skills that you learned from the old monk. However, the zombies start doing \nthe thriller dance and they begin to surround you. You try windmilling to try and intimidate them, but there's too many zombies. After \nthree days of non-stop dancing, you collapse onto the floor from exhaustion and the zombies eat you. \nTHE END");
                                                                break outerloop;
                                                            }
                                                            else{
                                                                System.out.println("Error. Enter one of the numbered options below.\n" + menu12);
                                                                menuOption=reader.nextLine();
                                                                System.out.println();
                                                            }
                                                        }
                                                    }
                                                    else{
                                                        System.out.println("Error. Enter one of the numbered options below.\n" + menu11);
                                                        menuOption=reader.nextLine();
                                                        System.out.println();
                                                    }
                                                }
                                            }
                                            else if(menuOption.equals("3")){
                                                menuOption="5";
                                                System.out.println("I guess you like zombies or something. You start selling Magikarp sushi and people start turning into zombies. Nice job. \nWhat do you choose to do?");
                                                System.out.println(menu9);
                                                menuOption=reader.nextLine();
                                                System.out.println();
                                            }
                                            else{
                                                System.out.println("Error. Enter one of the numbered options below.\n" + menu9);
                                                menuOption=reader.nextLine();
                                                System.out.println();
                                            }
                                        }
                                    }
                                    else{
                                        System.out.println("Error. Enter one of the numbered options below.\n" + menu6);
                                        menuOption=reader.nextLine();
                                        System.out.println();
                                    }
                                } 
                            }
                            else if(menuOption.equals("3")){
                                System.out.println("You live the chill life. You lay down in a grass field with the wind blowing through you hair. You look up in the sky and try picking \nout pictures in the clouds. You think you see your dead Pokemon Magikarp in the clouds when you hear a noise behind you. But you're chill. \nYou don't care. You get up and start running through the grass without a care in the world. Oh look! Isn't that the- too late. \nYOU JUST GOT BIT! \nTHE END");
                                break outerloop;
                            }
                            else{
                                System.out.println("Error. Enter one of the numbered options below.\n" + menu4);
                                menuOption=reader.nextLine();
                                System.out.println();
                            }
                        }
                    }
                    else{
                        System.out.println("Error. Enter one of the numbered options below.\n" + menu1);
                        menuOption=reader.nextLine();
                        System.out.println();
                    }
                }
            }
            else if(menuOption.equals("3")){
                menuOption="5";
                System.out.println("After wandering in the forest for a couple hours, you see a hotel and decide to stay for a night. You wake up the next morning \nfeeling refreshed. \nWhat do you choose to do?");
                System.out.println(menu2);
                menuOption=reader.nextLine();
                System.out.println();
                while(menuOption!="-1"){
                    if(menuOption.equals("1")){
                        System.out.println("You ain't no Superman, so you die. \nTHE END");
                        break outerloop;
                    }
                    else if(menuOption.equals("2")){
                        break;
                    }
                    else if(menuOption.equals("3")){
                        System.out.println("After watching a bunch of Adventure Time and taking a nap, you feel like going to the pool. There you challenge an old man with a cane \nto an underwater fistfight. You go in for the first punch but then the old man starts beating you with a cane. You then steal the cane \nand start beating him up. After five minutes, you realize that you killed him, so you proceed to stealthily exit the pool. You go back \nto your room to take a shower and then you watch some Food Network for five hours until you become bored again. \nWhat do you choose to do? \n" + menu2);
                        menuOption=reader.nextLine();
                        System.out.println();
                    }
                    else{
                        System.out.println("Error. Enter one of the numbered options below. \n" + menu2);
                        menuOption=reader.nextLine();
                        System.out.println();
                    }
                }
            }
            else{
                System.out.println("Error.Enter one of the numbered options below. \n" + menu);
                menuOption=reader.nextLine();
                System.out.println();
            }
        }
    }
}
