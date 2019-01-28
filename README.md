# Voting Methods - A Taxonomic List

## This should serve as a quick and easy reference for all voting methods.

## Some methods may appear multiple times as they fall under multiple categories.

##### Hyperlinks coming soon!

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <script src="http://code.jquery.com/jquery-1.10.1.min.js"></script>
  <script type="text/javascript">
    $(document).ready(function () {
      $('.close').slideUp().parent().children('span:first-child').css('text-decoration', 'underline');
      $('#election-method-list span').click(function (e) {
        $(this).parent().children('ul.open').removeClass('open').addClass('slideup').slideUp();
        $(this).parent().children('ul.close').removeClass('close').addClass('slidedown').slideDown();
        $('.slideup').removeClass('slideup').addClass('close').parent().children('span:first').css('text-decoration', 'underline');
        $('.slidedown').removeClass('slidedown').addClass('open').parent().children('span:first').css('text-decoration', 'none');
      });
    });
  </script>
  <title>List of Election Methods</title>
</head>

<body>
  <ul id="election-method-list">
    <li><span>Single-Winner Methods</span>
      <ul class="close">
        <li><span>Single-Choice</span>
          <ul class="close">
            <li><span>First Past The Post</span>
              <ul class="close">
                <li><span>First Past the Post</span></li>
                <li><span>Improved FPTP</span></li>
              </ul>
            </li>
            <li><span>Rounds</span>
              <ul class="close">
                <li><span>Top-Two</span></li>
              </ul>
            </li>
            <li><span>Asset Voting</span></li>
          </ul>
        </li>
        <li><span>Ranked (Preferential)</span>
          <ul class="close">
            <li><span>Pairwise (Condorcet)</span>
              <ul class="close">
                <li><span>Ranked Pairs (Tideman)</span></li>
                <li><span>Schulze</span></li>
                <li><span>Copeland</span></li>
                <li><span>Minimax</span></li>
                <li><span>Cardinal Pairwise (Cardinal Weighted Pairwise)</span></li>
                <li><span>Random Condorcet</span></li>
              </ul>
            </li>
            <li><span>Runoff Methods</span>
              <ul class="close">
                <li><span>Bucklin</span></li>
                <li><span>Coomb's</span></li>
                <li><span>IRV</span>
                  <ul class="close">
                    <li><span>IRV</span></li>
                    <li><span>Pairwise IRV</span></li>
                    <li><span>IRV-Check</span></li>
                    <li><span>BTR-IRV</span></li>
                    <li><span>Candidate Withdrawal IRV (CWO-IRV)</span></li>
                  </ul>
                </li>
              </ul>
            </li>
            <li><span>Borda Count</span></li>
          </ul>
          <li><span>Cardinal Methods</span>
            <ul class="close">
              <li><span>Approval</span>
                <ul class="close">
                  <li><span>Pure Approval</span>
                    <ul class="close">
                      <li><span>Approval Voting</span></li>
                      <li><span>Concensus Voting</span></li>
                      <li><span>Utilitarian Voting</span></li>
                    </ul>
                  </li>
                  <li><span>Disapproval Voting</span></li>
                  <li><span>Approval with Optional Conditional</span></li>
                  <li><span>Random Approval</span></li>
                </ul>
              </li>
              <li><span>Range (Score)</span>
                <ul class="close">
                  <li><span>Pure Score</span></li>
                  <li><span>STAR</span></li>
                </ul>
              </li>
              <li><span>Grades</span>
                <ul class="close">
                  <li><span>3-2-1 Voting</span></li>
                  <li><span>Majority Judgement</span></li>
                  <li><span>Disapproval Voting</span></li>
                  <li><span>Majority Choice Approval</span></li>
                </ul>
              </li>
            </ul>
          </li>
          <li><span>Hybrid Methods</span>
            <ul class="close">
              <li><span>Cardinal+Ranked</span>
                <ul class="close">
                  <li><span>Score+Ranked</span>
                    <ul class="close">
                      <li><span>Score+Condorcet</span>
                        <ul class="close">
                          <li><span>Score/DSV</span></li>
                          <li><span>Cardinal-Weighted Pairwise</span></li>
                        </ul>
                      </li>
                      <li><span>Definite Majority Choice</span></li>
                      <li><span>Marginal Ranked Approval Voting (MRAV)</span></li>
                    </ul>
                  </li>
                  <li><span>Approval+Ranked</span>
                    <ul class="close">
                      <li><span>Approval+Condorcet</span>
                        <ul class="close">
                          <li><span>Definite Majority Choice</span></li>
                          <li><span>Lull-Approval</span></li>
                          <li><span>Pairwise Sorted Approval</span></li>
                          <li><span>Approval Sorted Margins</span></li>
                        </ul>
                      </li>
                    </ul>
                  </li>
                </ul>
              </li>
              <li><span>Score+Graded</span>
                <ul class="close">
                  <li><span>Majority Acceptable Score</span></li>
                </ul>
              </li>
              <li><span>Condorcet+Borda</span>
                <ul class="close">
                  <li><span>Black's System</span></li>
                </ul>
              </li>
              <li><span>Pairwise Sorted Borda</span></li>
            </ul>
          </li>
          <li><span>Candidates Trade Votes</span>
            <ul class="close">
              <li><span>Asset Voting</span></li>
              <li><span>Optional Asset</span></li>
              <li><span>Cumulative Asset</span></li>
            </ul>
          </li>
          <li><span>Lottery Methods</span>
            <ul class="close">
              <li><span>Random Ballot</span></li>
              <li><span>Random Condorcet</span></li>
            </ul>
          </li>
      </ul>
      </li>
      <li><span>Multi-Winner Methods</span>
        <ul class="close">
          <li><span>Single-Choice</span></li>
          <li><span>Ranked</span>
            <ul class="close">
              <li><span>Single Transferrable Vote</span></li>
            </ul>
          </li>
          <li><span>Cardinal</span></li>
        </ul>
      </li>
  </ul>
</body>

</html>
	
	
		
				
			
				
##### Multi-Winner Methods Coming Soon!			
				
##### Don't see a voting method? Add it [here](https://docs.google.com/document/d/1J7eP_d6nccCDZYVWdtitqpXbW2a0VU9bluju91NCLt8/edit).
